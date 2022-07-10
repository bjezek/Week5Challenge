# Week5Challenge
# Imported Libaries import os(read file env)
import requests(pulls stock and bond info with api key)
import json(able to import database as json format)
import pandas as pd(financial liabries)
from dotenv import load_dotenv(Make sure file is loaded in system)
import alpaca_trade_api as tradeapi(pull up to date stock info with alpaca api & secret key)
from MCForecastTools import MCSimulation(run monte carlo simulation)
import matplotlib as plt (plot graph bar and histogram)
%matplotlib inline ( plot line graphs) 

# Calculate portfolio crypto, stock & bonds
calculated value of crypto, stock & bond portfolio mix based on its current value and 
added weight to a diversified portfolio first 40/60 then 20/80 to help determine growth
potential for a 30 year period vs a 10 year period seeing which one is more fiesable for retirment 
based on currrent investment strategies.

# The Big Picture
Plot graphs to see distribution probability of future returns based on passed events, used std from 30 year
to 10 year as well as plotting the confidence interval of returns based on current investment structure.

# See if your covered for emerginces !!!
creat if statements for scenarios in the portfoio to display to the user. 


if total_portfolio[0] > emergency_fund_value:
           print(f"Congratulations you have enough to cover you")
elif total_portfolio == emergency_fund_value:
       print(f" Congratulations you reached an important goal")
else:
       print(f"Your total portfolio is {(total_portfolio - emergency_fund_value)} away from your goal")
for user to see if emergency fund is less than total portfolio value then peace of mind is yours but if not 
you probably need to change investment strategy or not invest in the market due to risk factors at this time with 
limited cash reserves. 


# Monte_Carlo
After running 30 year 40/60 weight for AGG,SPY then a 10 year 20/80 weight it was clear to see more aggressive approach in having majority of 
capital in equites shows to be in the investors best interest based on growth compared to the more conservative profile based on std and probability of future returns. 
