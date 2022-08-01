# Bike Sharing System

Regression model for bike sharing dataset

Creating a regression model to predict number of bike rented in a certain day of a certain season

Video Explanation: [Youtube](https://youtu.be/_RPsJVi-USM)

***

Multicollinearity Test:
<html>
<body>
<!--StartFragment-->

variables | VIF
-- | --
weather | 3.856182
holiday | 1.031887
season | 3.913601
hour | 4.177052
count | 2.378707

<!--EndFragment-->
</body>
</html>

***

Final test result:
<html>
<body>
<!--StartFragment-->

Data| R2 | RMSE | MAE | MAPE
-- | -- | -- | -- | --
Train Score | 0.858177 | 68.242118 | 42.070198 | 0.356745
Test Score | 0.704922 | 98.452385 | 63.788331 | 0.658714

<!--EndFragment-->
</body>
</html>

***

Based on test result, model is still overfitted, and could be improved by:
- Add new feature(s) that better represent/ correlate with "count"
- Use a more complex model
- More feature engineering. For ex: binning categories in "hour", changing "temp" and "atemp" to a different scale, etc.
