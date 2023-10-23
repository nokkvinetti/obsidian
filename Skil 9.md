![[Pasted image 20231023094854.png]]
a)
Null hypothesis $H_0$: Resistance doesn't change under pressure, $\mu_0=\mu_1$
Alternative hypothesis $H_1$: Resistance changes under pressure,  $\mu_0 \not= \mu_1$ 
we will use a **paired t-test** since the order matters, as we are comparing each data point without pressure with it's correlating data point with pressure.

b) 
we use the R function t.test($\bar{x},\bar{y}$,Paired=TRUE) to perform a paired t test
from it we get that the p-value = 0.002744 < 0.05 so we reject the null hypothesis, and the resistance changes under pressure.


c) 
we get the 95% confidence interval of the mean resistance under pressure using the R function for one sample t test t.test($\bar{y}$)
we get that the 95%CI = (15.9, 16.1)

![[Pasted image 20231023101332.png]]

a)
null hypothesis $H_0$: the proportions of Collab-Nocco-monster are the same for all departments
alternative hypothesis $H_1$: the proportions are different, they depend on the department

we use the R function chisq.test(mat) and from it we get that the p-value=0.189 > 0.05 so we accept the null hypothesis.

b)
we find the chi-square test statistic that corresponds to the p-value=0.013 
using the R function qchisq(1 - p, DOF) where p is 0.013 and DOF is $($number of rows$-1)*($number of columns$-1)=4$
we get $\chi^2$=chisq(1 - p, DOF)=12.67107
so the value of the test statistic that corresponds to the p-value=0.013 is
$\chi^2$ = 12.7

![[graphchisquare]]
