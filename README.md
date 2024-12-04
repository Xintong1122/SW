# Campus Intelligent Web3 Ecosystem - Exploring Motivation Gaps and Web3 Incentives in Learning Communities
*Duke Kunshan University Signature Work 2025*

## Introduction

Motivation is one of the most crucial elements for successful learning, yet it is also one of the most difficult to sustain, especially in online learning communities. With the proliferation of online learning platforms and communities, learners are increasingly reliant on virtual spaces to seek support, accountability, and engagement. However, many traditional platforms lack structured systems to address long-term motivational challenges, leading to disengagement and inconsistent participation among users.

One prominent example is Study Together, one of the largest study and productivity communities on Discord. The platform provides a space for learners to connect, share experiences, and support each other, with its #motivation channel serving as a hub for discussions about learning challenges, strategies, and successes. While Study Together thrives on peer-driven interactions, the absence of formal mechanisms for incentivizing engagement often leaves gaps in motivation. Users frequently discuss issues such as maintaining study consistency, dealing with distractions, and staying productive over extended periods, which points to the need for more effective and innovative approaches to foster engagement.

In parallel, emerging Web3 technologies offer promising solutions for reimagining educational incentives. By leveraging blockchain, decentralized platforms introduce token-based reward systems, community-driven governance, and immutable skill certification to enhance user engagement. A leading example is UDAO, a Web3-powered learning platform launched in June 2024 by a team of experts from ETH Zurich. UDAO integrates gamified rewards through ERC-20 tokens, blockchain-based skill validation, and a governance model that allows community members to shape the platform’s evolution. By rewarding users for their participation and achievements, UDAO aims to create a self-sustaining ecosystem where learning is both incentivized and decentralized.

Despite its innovative features, the effectiveness of UDAO’s incentive mechanisms remains underexplored. Initial analysis of UDAO’s tokenomics reveals challenges, including declining token prices and trading volumes, which may indicate issues with its economic design and its ability to sustain long-term engagement. Similarly, user feedback from UDAO’s #suggestion channel highlights areas for improvement in reward mechanisms, platform usability, and governance features. These insights raise critical questions about the role of Web3 in addressing motivational challenges and the extent to which such platforms can fulfill their potential as transformative tools for education.

This study aims to bridge the gap between traditional and Web3-enabled learning systems by examining motivational challenges in traditional platforms and evaluating the effectiveness of Web3 incentive mechanisms. By analyzing data from Study Together and UDAO, this research will identify key gaps in user motivation, evaluate the strengths and weaknesses of token-based reward systems, and propose advanced mechanisms for creating sustainable, engaging, and learner-focused ecosystems. Through this exploration, the study seeks to contribute to the growing field of Web3 education and offer actionable insights for designing improved incentive models that address the evolving needs of learners.


## Research Questions

- **RQ1:** What are the key motivational challenges faced by users in traditional learning communities such as Study Together?
- **RQ2:** How can newly developed Web3 study platforms such as UDAO’s incentive mechanisms effectively address these challenges?

## Data

### **Meta Data Information**

**1. UDAO Daily Data**

The first dataset consists of daily price and volume data for the UDAO token, downloaded directly from CoinMarketCap. The dataset includes fields such as opening price, closing price, daily high, daily low, trading volume, and timestamp. It provides a comprehensive view of UDAO's market performance and was retrieved from the official UDAO page on CoinMarketCap: *https://coinmarketcap.com/currencies/udao/*.

**2. User Messages from Discord Channels**

The second dataset comprises user messages extracted from two Discord channels.The data was collected using the open-source tool DiscordExplorer: *https://github.com/mdawsonuk/DiscordExplorer*. This dataset includes message content, timestamps, and user sentiment, enabling both sentiment and topic analysis.
- The #motivation channel in the Study Together Discord community, focusing on discussions about learning motivation and challenges.
- The #suggestion channel in the UDAO Official Discord server, where users provide feedback and suggestions regarding the UDAO platform. 

### **Data Dictionary**

#### **Dataset 1: UDAO Daily Market Data**

| **Variable Name**  | **Description**                                           | **Frequency** | **Unit**         | **Type**      |
|---------------------|-----------------------------------------------------------|---------------|------------------|---------------|
| Name               | The identifier for the dataset entry                      | Daily         | Numeric          | Identifier    |
| Open               | The opening price of UDAO for the day                     | Daily         | USD              | Numeric       |
| High               | The highest price of UDAO for the day                     | Daily         | USD              | Numeric       |
| Low                | The lowest price of UDAO for the day                      | Daily         | USD              | Numeric       |
| Close              | The closing price of UDAO for the day                     | Daily         | USD              | Numeric       |
| Volume             | The total trading volume of UDAO for the day              | Daily         | USD              | Numeric       |
| MarketCap          | The market capitalization of UDAO for the day             | Daily         | USD              | Numeric       |
| Timestamp          | The date and time the record was logged                   | Daily         | ISO8601 Timestamp| Timestamp     |

---

#### **Dataset 2: User Messages from Discord Channels**

| **Variable Name**  | **Description**                                           | **Frequency** | **Unit**         | **Type**      |
|---------------------|-----------------------------------------------------------|---------------|------------------|---------------|
| AuthorID           | The unique identifier of the message author               | Per message   | Numeric ID       | Identifier    |
| Author             | The username of the message author                        | Per message   | String           | Categorical   |
| Date               | The date and time the message was posted                  | Per message   | ISO8601 Timestamp| Timestamp     |
| Content            | The textual content of the message                        | Per message   | Text             | Text          |
| Attachments        | Any attachments included in the message                   | Per message   | File Links       | Text          |
| Reactions          | Emoji reactions to the message, including counts          | Per message   | Emoji + Count    | Categorical   |


## Code

### **Code Description**

| **Section**              | **Description**                                                                                                    |
|--------------------------|--------------------------------------------------------------------------------------------------------------------|
| **Price**   | Calculates representative prices, daily percentage changes, and visualizes price trends and trading volumes.      |
| **Data Loading and Cleaning**   | Processes message content, timestamps, and reactions for sentiment and topic modeling.                            |
| **UDAO Suggestion**       | Word Frequency Analysis.                                                   |
|                          | Topic Analysis.                                         |
|                          | Network Analysis.                                           |
| **Study Together Motivation**       | Word Frequency Analysis.                                                   |
|                          | Topic Analysis.                                         |
|                          | Network Analysis.                                           |

## Insights

### Study Together Community Motivation

<p align="center">
  <img src="Figure/w2.png" alt="Sample Image" width="500"/>
</p>
<p align="center">
  <em>Figure 1: Word Frequency in Study Together.</em>
</p>

<p align="center">
  <img src="Figure/l2.png" alt="Sample Image" width="500"/>
</p>
<p align="center">
  <em>Figure 2: Topic Analysis in Study Together.</em>
</p>

<p align="center">
  <img src="Figure/n2.png" alt="Sample Image" width="500"/>
</p>
<p align="center">
  <em>Figure 3: Network Analysis in Study Together.</em>
</p>


### UDAO Community Tokenomics

<p align="center">
  <img src="Figure/p1.png" alt="Sample Image" width="500"/>
</p>
<p align="center">
  <em>Figure 4: UDAO Token Daily Representative Price Trend.</em>
</p>

<p align="center">
  <img src="Figure/p2.png" alt="Sample Image" width="500"/>
</p>
<p align="center">
  <em>Figure 5: UDAO Token Trading Volume Trend.</em>
</p>

<p align="center">
  <img src="Figure/p3.png" alt="Sample Image" width="500"/>
</p>
<p align="center">
  <em>Figure 6: UDAO Token Daily Percentage Change Distribution.</em>
</p>

### UDAO Community Suggestion

<p align="center">
  <img src="Figure/w1.png" alt="Sample Image" width="500"/>
</p>
<p align="center">
  <em>Figure 7: Word Frequency in UDAO.</em>
</p>

<p align="center">
  <img src="Figure/l1.png" alt="Sample Image" width="500"/>
</p>
<p align="center">
  <em>Figure 8: Topic Analysis in UDAO.</em>
</p>

<p align="center">
  <img src="Figure/n1.png" alt="Sample Image" width="500"/>
</p>
<p align="center">
  <em>Figure 9: Network Analysis in UDAO.</em>
</p>

## Author Information 
- **Author:** Xintong Wu, majoring in Computation and Design/ Computer Science, Duke Kunshan University, Class of 2025.
- **Mentors:** Prof. Luyao Zhang, Duke Kunshan University.

## Resources

- https://udao.org/



