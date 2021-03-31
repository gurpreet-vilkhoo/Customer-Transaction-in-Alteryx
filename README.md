## Customer-Transaction-in-Alteryx
Using in-built sample data of customer transactions and preparing data flow in Alteryx Designer

### Objective- To classify the customers into groups based on amount spend and number of visits

### About dataset

The data consists of 2669 records with the following columns:

![image](https://user-images.githubusercontent.com/80466173/113136312-db50cd00-9240-11eb-88b0-220af3770762.png)


### Calculating column containing standard deviations of visits using Tile in Preparation(Tile_Num)

![image](https://user-images.githubusercontent.com/80466173/113137126-bdd03300-9241-11eb-985d-376c62ebb3e1.png)


### Renaming Tile_Num to Visit_Group and removing column "Tile_SequenceNum

![image](https://user-images.githubusercontent.com/80466173/113137460-33d49a00-9242-11eb-8322-367afff2d0b8.png)

### Similarly create Tile for Spend and Renaming Tile_Num to Spend_Group and removing column "Tile_SequenceNum

![image](https://user-images.githubusercontent.com/80466173/113137912-c5dca280-9242-11eb-994c-41d95d0c8991.png)


