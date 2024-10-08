This repository contains code for estimating **Li-ion cell parameters** using data from **EIS** testing.

I have uploaded the dataset used in _EIS.txt_

I have used a ***1RC*** model with ***Warburg*** impeadance to fit our _nyquist_ plot.
![screen shot of 1RC model with warburg impadance.](https://github.com/user-attachments/assets/8180ba6f-f52e-4d7f-b24a-4f9aa5a7ce10)

Expected nyquist plot for ***1RC** model with ***Warburg*** impeadance looks like
![screenshot of expexted model.](https://github.com/user-attachments/assets/c15b131a-d7b4-4b71-bace-a0a53970ca7c)


# NYQUIST PLOT
Nyquist plots are polar plots for finding the stability of the closed loop control systems by varying ω from −∞ to ∞.
The **X-axis** represents the **Real part** of the complex transfer function.
The **Y-axis** represents the **imaginary part**.
Here we use nyquist plot to choose our equivalent circuit.

# METHODOLOGY

Here I have used multivariate regression model to estimate our _four_ cell parameters. As a thumb rule I have made sure that the **_RMSE_** error is less than 2%.
The number of iterations used can be changed according to the error. PyTorch library is used here to implement the regression model.

