# Stock Analysis Script Analysis

  We recently created a stock analysis program for a client that would analyze stock performance over time to find good investment opportunities. We created a version 1.0 of the script which performed as desired, but could have struggled to run through very large datasets in a reasonable amount of time. We set out to create a version 2.0 of the Stock Analysis script which would perform the same function, but more efficiently, so it could be effectively deployed to analyze many more stocks at once. We then analyzed the results here.
  
## The Times

  The results of our code refactoring were quite successful. The updated code performs the same task 8 times quicker then the original code. Verison 1.0 code processed our initial dataset in an average of 0.8 seconds.
  
![VBA_Module_2017](https://github.com/coryknuth/stock-analysis/blob/b239102ab29b09b7133fe40d34ce42a430a375a1/Resources/VBA_Module_2017.png) ![VBA_Module_2018](https://github.com/coryknuth/stock-analysis/blob/b239102ab29b09b7133fe40d34ce42a430a375a1/Resources/VBA_Module_2018.png)

  After code refactoring the performance of the code improved to an average of around 0.1 seconds for the same dataset.
  
  ![VBA_Challenge_2017](https://github.com/coryknuth/stock-analysis/blob/b239102ab29b09b7133fe40d34ce42a430a375a1/Resources/VBA_Challenge_2017.png) ![VBA_Challenge_2018](https://github.com/coryknuth/stock-analysis/blob/b239102ab29b09b7133fe40d34ce42a430a375a1/Resources/VBA_Challenge_2018.png)
  
  
