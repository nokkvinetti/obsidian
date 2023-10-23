T-302-TOLF
Nökkvi Marz Þórleifsson
# Vika 1
![[Pasted image 20231023141616.png]]
we use R to calculate 
mean(Data)= 6.596452 ~ 6.60
median(Data)=5.75 
sd(Data)=4.518998 ~4.52
we use the function hist(data,breaks=4) to get a histogram with 4 breaks
![[Pasted image 20231023143524.png]] 
we change the number of breaks to 6 for the histogram with 6 breaks
![[Pasted image 20231023144205.png]]
and change again for the 8 breaks
![[Pasted image 20231023144234.png]]
we use the function boxplot(Data,main="box plot of Data") to plot a boxplot of our data
![[Pasted image 20231023144946.png]]

#### 1.2
![[Pasted image 20231023150029.png]]

The median will always equal one of the values of the sample if the sample size is an odd number because the median is the middle number for example 1, 2, 3, 4, 5 is an odd number sample size therefore 3 is the median however if we had 1,2,3,4,5,6 the median would be 3.5.

![[Pasted image 20231023150106.png]]

The standard deviation is always equal to or less than the mean. The formula for standard deviation subtracts each data point from the mean; because it is squared, it’s impossible for it to be more; when every value is positive.

![[Pasted image 20231023150129.png]]

Yes, it is possible for the standard deviation of a list to equal 0, when you have a list of the same number the standard deviation will be 0, because the mean will equal the number.

![[Pasted image 20231023150224.png]]

If you give every worker a 50-dollar raise a week, It will raise the mean salary by 50 for example:

( 4+5+6+7+5 )/ 5 = 5.4 
And after giving everyone a 50-dollar raise
( 4+(50)+5+(50)+6+(50)+7+(50) +5 + (50) ) / 5 = 55.4

since giving everyone a 50 dollar raise only shifts the distribution by 50 
the standard deviation would remain unchanged

  

![[Pasted image 20231023150813.png]]

If everyone got a 5% raise in another company, it would raise the mean salary by 5% for example:
( 4+5+6+7+5 )/ 5 = 5.4 
After giving a 5% (1.05) raise 
1.05( 4+5+6+7+5 )/ 5 = 5.67
and it would raise the standard deviation by 5% 
as you would multiply every data point by 1.05

![[Pasted image 20231023165527.png]]
a)Find the sample mean number of occupants.

$\bar{x}=\frac{1}{n}\sum^{n}_{i=1}x_i$
$\bar{x}=\frac{1}{100}(1*70+2*15+3*10+4*3+5*2)=1.52$

b)Find the sample standard deviation of the number of occupants.
$S=\sqrt{\frac{1}{n-1}\sum^{n}_{i=1}(x_i-\bar{x})^2}$
$S$=$\sqrt{\frac{1}{99}(70*(1-1.52)^2+15*(2-1.52)^2+10*(3-1.52)^2+3*(4-1.52)^2+2*(5-1.52)^2)}$=0.937

c)Find the sample median number of occupants.
the median number of occupants is 1 since the median is the middle number and we have 70 cars with 1 occupant

d)Compute the first and third quartiles of the number of occupants.
we use the R function quantile to calculate the quartiles of the number of occupants
first quartile: quantile(occupants,0.25)= 1
and  third quartile: quantile(occupants,0.75)=2


e)What proportion of cars had more than the mean number of occupants?
P(x>$\bar{x}$)=$\frac{15+10+3+2}{100}=0.30$
30% of cars had more than 1.52 occupants

f)For what proportion of cars was the number of occupants more than one standard deviation greater than the mean?
P(x>$\bar{x}+S$)=$\frac{10+3+2}{100}=0.15$
15% of cars had more than 2.46 occupants

g) For what proportion of cars was the number of occupants within one standard deviation of the mean?
P(x<$\bar{x}+S$)=$\frac{70+15}{100}=0.85$

#### 1.3
![[Pasted image 20231023174431.png]]
a) it's closest to 30%
b) there are more men in the interval 240-260 mg/dL

#### relation between sample variance and mean values
equation 1.2: $S^2=\frac{1}{n-1}\sum^{n}_{i=1}(x_i-\bar{x})^2$
equation 1.3: $S^2=\frac{1}{n-1}(\sum^{n}_{i=1}{x_i}^2-n\bar{x}^2)$
$S^2 \approx (\bar{x^2})-(\bar{x}^2)$

#### 2.1
![[Pasted image 20231023183625.png]]
a)Find a sample space for this experiment.
we find the sample space = (1,1,1,2,2,3)

b)Find P(odd number).
since we have 4 odd numbers out of 6 numbers
P(odd number)=4/6 = 66.67%

c)If the die were loaded so that the face with the 3 on it were twice as likely to come up as each of the other five faces, would this change the sample space? Explain.
the sample space does not change because loading the die changes the probabilities, but not the outcomes. So, the sample space, which is the set of all possible outcomes, remains the same


d)If the die were loaded so that the face with the 3 on it were twice as likely to come up as each of the other five faces, would this change the value of P(odd number)? Explain.
yes the value of P(odd number) would change as the probability of getting 3 has doubled
P(odd number with 3 double as likely)=p(1)+p(3)=$1/6*2+3/6=5/6=83.33$


![[Pasted image 20231023183646.png]]
a)List all 16 outcomes in the sample space.
1.TTTT 2. TTTF 3. TTFT 4. TTFF 5. TFTT 6. TFTF 7. TFFT 8. TFFF 9. FTTT 10. FTTF 11. FTFT 12. FTFF 13. FFTT 14. FFTF 15. FFFT 16. FFFF)

b)Assuming the outcomes to be equally likely, find the probability that all the answers are the same.
P(all answers same)=p(all answers True)+p(all answers false)=2/16= 1/8

c)Assuming the outcomes to be equally likely, find the probability that exactly one of the four answers is “True.”
4* 1/2

d) Assuming the outcomes to be equally likely, find the probability that at most one of the four answers is “True.”
5/16

![[Drawing 2023-10-23 23.17.10.excalidraw]]

<div style="page-break-after: always;"></div>
# Vika 2
<div style="page-break-after: always;"></div>
# Vika 3
<div style="page-break-after: always;"></div>
# Vika 4
<div style="page-break-after: always;"></div>
# Vika 5
<div style="page-break-after: always;"></div>
# Vika 6
<div style="page-break-after: always;"></div>
# Vika 7
<div style="page-break-after: always;"></div>
# Vika 8

#### 5.1

![[Pasted image 20231018180051.png]]

![[Pasted image 20231018180412.png]]

#### 5.7
![[Pasted image 20231018180558.png]]

#### 5.7
![[Pasted image 20231018180656.png]]

#### 6.1
![[Pasted image 20231018184231.png]]
$\mu=15, n=86, S=1.8, \bar{x}=15.2$ 
$H_0:\mu=15$ the supposed mean diameter is right
$H_0:\mu\not=15$ the supposed mean diameter is wrong

a) lets find the P-value using Z score
$\sigma_\bar{x}=\frac{S}{\sqrt{n}}=\frac{1.8}{\sqrt{86}}$=0.1941
$Z=\frac{\bar{x}-\mu}{\sigma_\bar{x}}=\frac{0.2}{0.1941}=1.03$
we plug the z score into R and get
P=2$*$pnorm(-1.03,0,1)=0.30

b)I believe it's plausible as we get P=0.30 which is higher than 0.05 so the null hypothesis is possible

![[Pasted image 20231018184312.png]]

#### 6.4
![](https://lh7-us.googleusercontent.com/IHWgWEYLUp1Wbx3sYky23INEnrTvDe4W5S--Bs2uHaWxTnKJD4Z3RFcATBqn7GWIHVE_Htw1mid6I_anZ3pm7HcxeYF-cWTTMr69pQt1zQZRjsnk2xEWvgOzaDYaREbqD-_edYc7OIBq7OOJR2WS9SU)

![](https://lh7-us.googleusercontent.com/bz2PY0gPMcW8z0izO5nv9R8qNl3Uz4mOcVARNUuzsN1y4l_rT8Y2pevNtbJHVuyd6N1cyAo1Uc_L2lsUtjUecz55BOo9uAFEA3XGKmraa42M5er1KzmDvy9LxdOh9eBfTVp4kCk7NI4UT4ZlgyxHPg8)









<div style="page-break-after: always;"></div>
# Vika 9
<div style="page-break-after: always;"></div>
# Vika 10
<div style="page-break-after: always;"></div>
# Vika 11
<div style="page-break-after: always;"></div>
# Vika 12



