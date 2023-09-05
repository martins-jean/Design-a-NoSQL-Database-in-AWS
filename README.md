# Design a NoSQL Database in AWS
Improved data access performance by creating a global secondary index in Amazon DynamoDB.

## Architecture Diagram

![Screenshot 2023-09-04 at 19 31 15](https://github.com/martins-jean/Design-a-NoSQL-Database-in-AWS/assets/118685801/36df7d16-c24f-4060-bc75-a008fa7bb0e5)

## Project Overview

1. Amazon DynamoDB design should be governed by the data access pattern. Every read and write that is made to a DynamoDB table has its Read usage or Write usage computed. <br>
2. In this solution, indexes provide access to alternate query patterns, which you can use to speed up queries. After you create an index, the database maintains it for you. <br>
3. A global secondary index (GSI) contains a selection of attributes from the base table, but they are organized by a primary key that is different from that of the table. <br>
4. Using the badge-game-index GSI, you can quickly access the data of all players with specific badges, sorted by game. <br>
5. Using the games-top-scores GSI, you can quickly access the data of all top scores per game, sorted by score. <br>
6. Whether you are using a relational database or the DynamoDB NoSQL database service, you should be careful with index creation. <br>
7. Whenever a table write occurs, all of the table's indexes must be updated. In a write-heavy environment with large tables, this can consume large amounts of system resources. <br>

## Reproducibility Guidelines

<details>
  <summary>Required setup</summary>
  1. Create a DynamoDB table called "player_score" with sample game leaderboard data: <br>
  - Sort key: game_timestamp (number). <br>
  - Partition key: player_name (string). <br>
  - Capacity mode: on-demand. <br>
</details>

<details>
  <summary>Review the Amazon DynamoDB table structure</summary>
  1. Navigate to the DynamoDb console and click on the table you created. <br>
  2. Click 
</details>

<details>
  <summary>Compare the Scan and Query Operations</summary>
</details>

<details>
  <summary>Explore the filter expression and limit parameters</summary>
</details>

<details>
  <summary>Create a global secondary index (GSI) to optimize the search</summary>
</details>

<details>
  <summary>Compare the query performance using the created GSI</summary>
</details>
