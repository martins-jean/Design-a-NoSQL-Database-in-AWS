# Design a NoSQL Database in AWS
Improved data access performance by creating a global secondary index in Amazon DynamoDB.

## Architecture Diagram

![Screenshot 2023-09-04 at 19 31 15](https://github.com/martins-jean/Design-a-NoSQL-Database-in-AWS/assets/118685801/36df7d16-c24f-4060-bc75-a008fa7bb0e5)

## Project Overview

1. Amazon DynamoDB design should be governed by the data access pattern. Every read and write that is made to a DynamoDB table has its Read usage or Write usage computed. <br>
2. In this solution, indexes provide access to alternate query patterns, which you can use to speed up queries. After you create an index, the database maintains it for you. <br>

## Reproducibility Guidelines
