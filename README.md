## Classification of Customers into High and Low on basis of transactions
Using in-built sample data of customer transactions and preparing data flow in Alteryx Designer

#### Objective- To classify the customers into groups based on amount spend and number of visits

#### -About dataset

The data consists of 2669 records with the following columns:

![image](https://user-images.githubusercontent.com/80466173/113136312-db50cd00-9240-11eb-88b0-220af3770762.png)


#### -Calculating column containing standard deviations of visits using Tile in Preparation(Tile_Num)

![image](https://user-images.githubusercontent.com/80466173/113137126-bdd03300-9241-11eb-985d-376c62ebb3e1.png)


#### -Renaming Tile_Num to Visit_Group and removing column "Tile_SequenceNum

![image](https://user-images.githubusercontent.com/80466173/113137460-33d49a00-9242-11eb-8322-367afff2d0b8.png)

#### -Similarly create Tile for Spend and Renaming Tile_Num to Spend_Group and removing column "Tile_SequenceNum

![image](https://user-images.githubusercontent.com/80466173/113137912-c5dca280-9242-11eb-994c-41d95d0c8991.png)

#### -Create formula with condition such that if standard deviation of Spend_Group and Visit_Group is greater than 3, then label the target variable as "High" otherwise "Low"

![image](https://user-images.githubusercontent.com/80466173/113144818-50c19b00-924b-11eb-9cdc-f1dcbf2e47e2.png)


![image](https://user-images.githubusercontent.com/80466173/113144866-60d97a80-924b-11eb-8984-c8b8f8e442e4.png)


#### -Observation: There are large number of lows in the dataset(2618 vs 51) i.e. standard deviation is less than 3

![image](https://user-images.githubusercontent.com/80466173/113145533-291f0280-924c-11eb-9de6-c384374d0e5a.png)

![image](https://user-images.githubusercontent.com/80466173/113145586-39cf7880-924c-11eb-9cde-d30bb0035568.png)



#### -Final Designer flow

![image](https://user-images.githubusercontent.com/80466173/113145683-58357400-924c-11eb-918f-362e15b07cb0.png)

