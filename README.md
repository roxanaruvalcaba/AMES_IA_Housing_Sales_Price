# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 2: AMES, IA Housing Sales Price



### Problem Statement
We have 81 features related to housing sold in Ames, IA. I have been tasked with using this data to create a model that will predict the sales price of Ames housing. I can use as many or as few features as I like keeping in mind that I don’t want to over or under fit the model.


### Executive Summary
The results provided by my Lasso Model could be improved. The higher R2 value on the train vs test data leads me to believe there is high variance (overfit). Though Lasso helps reduce variance, it does not completely eliminate it. The other two models I looked at where the ridge model and linear regression. In terms of R2, I did not see a big difference in performance. The difference was noted when submitting the data to Kaggle. I believe this to be the case because the model has high variance. I chose the Lasso model as my final model because the Lasso model is the only one that zero's out coefficients. My findings were that the variables with high correlation had the highest contribution to price. Other findings are available in the Conclusion section below.

### Conclusion
There is a lot more I would want to do with additional time such as try and reduce the high variance. From my current model, I can conclude that the best neighborhood is Crawford for higher price housing. To improve selling price, owners can can improve material and finish quality. Overall, ground living area was the most important feature and none of the features included in the model reduced the value of housing.

### Next Steps
As next steps, I would further refine the model to lower variance. I would simplify the model by removing columns. I would begin removing columns by comparing p-values and coefficients. In addition, I would look into external research to see what other important factors should be added that are not already in the model.

### Contents

- [PPT](./AMES_Sales_Prie_PPT.pdf)
- [Code](./code)
- [Train Data](./datasets/train.csv)
- [Test Data](./datasets/test.csv)
- [Kaggle Sales Price](./datasets/submit_7.csv)

The train data includes information from 2,051 sales which have 81 detailed features. The selling price time frame is from 2006 to 2010. The test data provides information for 878 houses for us to predict the selling price, but does not provide the selling price. Both the code and datasets folders have an archive folder of draft information.

### Additional

External research shows that there are many factors both macro and micro that affect housing prices. For example, there was a fall of the market in 2008 that can be visualized by the year sold data. The economy is an important factor in housing prices. In addition, there are other factors that affect housing prices such as location. This includes the school ratings, how close a house is to entertainment, whether or not there are jobs near the house, and more. Interest rates and incentives will also affect housing prices. There are many more details about factors that affect housing prices that are not included in the model. I have just mentioned a few.

