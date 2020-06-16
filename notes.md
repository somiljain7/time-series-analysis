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

