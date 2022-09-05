# Analyzing Green stocks with VBA

## Overview of Project
Steve just graduated with a finance degree and he wants to help his parents with stock investments. They are passionate about green energy and they have decided to invest all their money into DAQO New Energy Corporation. Steve, not willing to invest all the money in one stock. He believes funds should be more diversified and has asked us to look through several other green energy stocks along with DAQO stock.

### Purpose
The purpose of this project was to refactor the code. Present code works fine with dozens of stocks but in future it should work well with thousands of stocks. We need to refactor the original VBA code and it should successfully run faster. Developed VBA scripts to analyze the data for 2017 and 2018 years. Gained the below knowledge in VBA -

* Loops
* Operators 
* Arrays
* Popups
* Conditional Formatting
* Code refactoring

## Results
After performing analysis for 2017 and 2018 data, observed ENPH is performing well. 

![Stocksdata](https://user-images.githubusercontent.com/44387918/188414538-1c04f674-ed8b-4271-88bf-b2b8102e6017.png) 

Great difference observed in execution performance after refactoring the VBA code. 

Initial run took about 0.66 second: 
  
![VBA_Challenge_2018 copy](https://user-images.githubusercontent.com/44387918/188415909-ed6672dd-778c-49d9-b138-4807aeb205d3.png)

Refactored code just took 0.14:

![VBA_Challenge_2018](https://user-images.githubusercontent.com/44387918/188416258-65550356-d957-43f2-bb85-10554d0beb4a.png) 
 
Which is a great improvement in terms of execution performance. 

The initial code has nested for loops and the outer loop traverses 12 rounds for each ticker. 

![Screen Shot 2022-09-05 at 2 41 37 AM](https://user-images.githubusercontent.com/44387918/188419599-1a1fa9c2-f790-4c6b-88a4-5747afbf5250.png) 

The refactored code loop through all the data one time and stores the information. 

![Screen Shot 2022-09-05 at 2 48 09 AM](https://user-images.githubusercontent.com/44387918/188420791-da7d853c-c31c-4800-97e3-49fcda6e7e11.png) 

## Summary
Refactoring helps make our code cleaner and improve performance. Carrying out a series of small changes to the code base that are minor enough to avoid introducing new errors. Minor changes make code slightly better and the application is in  working state. However, it’s risky to refactor the code if we do not understand the code coverage properly. 

Original VBA script is simple and easily understandable. However, nested loops consume a lot of time. In general, we always need to minimize the nested loops to increase the performance in execution. Refactored script along with arrays is faster and loops through all the data one time in order to collect the same information as the original script. 



