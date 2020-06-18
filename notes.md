# notes
#  python packages to perform regression 

1)in statsmodels.api as sm
sm.OLS(y,x).fit()

2)in numpy 
np.polyfit(x , y ,   deg=1)

3)in pandas 
pd.ols ( y ,  x )

4)in scipy
from scipy import stats 
stats.linregress(x,y)


# correlation=sqrt(Rsquare)
# Autocorrelation is corr of a single time series with a lagged copy of itself
# with financial time series when returns have a negative autocorrelation it is mean reverting for vice versa condition trend following
# plot_acf is statsmodels function for plotting the autocorrelation function
input x is a series or array
lags = how many lags of the autocorrelation function will be plotted
alpha sets width of confidence interval 

# to_datetime() is used to convert an index often read in as a string into a datetime index
# df,index = pd.to_datetime(df.index)
changing an index to datetime

# joining two dateframes
df1.join(df2)
# computing percent changes and differences of a time series
df['col'].pct_change()
df['col'].diff()
# pandas correlation method of series
df['abc'].corr(df['xyz'])
# correlation coefficient is ameasure of how much two series vary together
# The positive correlation
means that when interest rates go down, stock prices go down. For example, during crises like 9/11, investors sold stocks and moved their money to less risky bonds (this is sometimes referred to as a 'flight to quality'). During these periods, stocks drop and interest rates drop as well. Of course, there are times when the opposite relationship holds too.

# A first step when analyzing a time series is to visualize the data with a plot. 

# Autoregressive integrated moving average model (ARIMA)
An Arima model is a class of statistical models for analyzing and forecasting time series data.
