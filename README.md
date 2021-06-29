# Stock Script Analysis

  We recently created a stock analysis program for a client that would analyze stock performance over time to find good investment opportunities. We created a version 1.0 of the script which performed as desired, but could have struggled to run through very large datasets in a reasonable amount of time. We set out to create a version 2.0 of the Stock Analysis script which would perform the same function, but more efficiently, so it could be effectively deployed to analyze many more stocks at once. We then analyzed the results here.
  
## The Times

  The results of our code refactoring were quite successful. The updated code performs the same task 8 times quicker then the original code. Verison 1.0 code processed our initial dataset in an average of 0.8 seconds.
  
![VBA_Module_2017](https://github.com/coryknuth/stock-analysis/blob/b239102ab29b09b7133fe40d34ce42a430a375a1/Resources/VBA_Module_2017.png) ![VBA_Module_2018](https://github.com/coryknuth/stock-analysis/blob/b239102ab29b09b7133fe40d34ce42a430a375a1/Resources/VBA_Module_2018.png)

  After code refactoring the performance of the code improved to an average of around 0.1 seconds for the same dataset.
  
  ![VBA_Challenge_2017](https://github.com/coryknuth/stock-analysis/blob/b239102ab29b09b7133fe40d34ce42a430a375a1/Resources/VBA_Challenge_2017.png) ![VBA_Challenge_2018](https://github.com/coryknuth/stock-analysis/blob/b239102ab29b09b7133fe40d34ce42a430a375a1/Resources/VBA_Challenge_2018.png)
  
  This drastic improvement would be critical if we were to analyze significantly larger datasets. Let's now look at both how we acheived this with our code, and some of the general advantages and disadvantages of doing this type of refactoring on this and other projects.
  
## The Factors of Refactor
  
  In this instance we were very successful in improving the efficiancy and simplicity of our code. While refactoring can be generally considered a good choice to get the most out of some already written code, there are, as with all things, costs and benefits to consider. Code refactoring does of course carry some risk of introducing new bugs into the code, which is a particular concern if you are considering refactoring code which is already completed, well tested, and stable. Refactoring can be time and cost intensive and should be handled carefully if deadlines are approaching or budget limits are close. These are many of the possible dangers from code refactoring, and should be considered in any case where refactoring is being considered for a project however there are many benefits which make choosing to refactor a potential win.
  
  First, refactoring allows a chance for peer review of your code. A second set of eyes is a huge potential win for any project combining the experience and style of multiple members of the team can elevate a piece of code to more than the sum of it's parts. Peer refactoring or even self refactoring also has a good chance of drastically improving the efficiency, and cleanliness of the code. With the proper time and care, refactoring can always lead to improvement in your code's total effectiveness. It is an excellent way to eliminate common problems in first drafts of code like duplicate or inefficient structures and methods. 
  
  In our stock analysis code we started by using a nested for loop to process each row of data. 
  
  ![VBA_Module_Code](https://github.com/coryknuth/stock-analysis/blob/c66f279e7aa345df8a20e9e6837526f34d5acdc2/Resources/VBA_Module_Code.png)
  
  This did prove to be effective as shown above. We were able to process the data still in under a second. It's relatively easy to understand and edit this code as well. However in our refactoring we were able to eliminate the nested for loop and accomplish the same outcome. By removing the nested loop we eliminated the exponential and duplicate processing that wasn't needed for this application. Here is a portion of the refactored code which eliminates the nested loop, is generally structured to be more modular and simple to understand, and accomplishes the same result in one-eighth the time.
  
  ![VBA_Challange_Code](https://github.com/coryknuth/stock-analysis/blob/c66f279e7aa345df8a20e9e6837526f34d5acdc2/Resources/VBA__Challenge_Code.png)
  
  In summary, our code refactoring as demonstrated above, was a big success for this project. The version 2.0 code will be much more effective and efficient at analyzing significantly larger datasets in the future. 
