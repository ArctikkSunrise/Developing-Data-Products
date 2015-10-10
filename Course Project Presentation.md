Course Project Presentation 
========================================================
author: KK
date: Sat Oct 10 19:24:19 2015    
font-family: 'Helvetica'


Calulation Formula
========================================================
The formula for calculating body fat is gender specific. To calculate body fat, the following inputs are required.

1. Weight (Kg)
2. Height (cm)
3. Age 
4. Gender: femail - gender = 0, mail - gender = 1

Calulation Formula (cont'd)
========================================================

First we calculate the body mass index, BMI

BMI = Weight(Kg)/(Height(m) x Height(m))

Then, use BMI to calculate body fat

Body fat (%) = (1.20 x BMI) + (0.23 x age) - (10.8 x gender) - 5.4


Description of percentage of body fat
========================================================


```
    Description  Female    Male
1 Essential fat    <15%     <5%
2      Athletes 15%-20%  5%-13%
3       Fitness 20%-24% 13%-17%
4    Acceptable 24%-31% 17%-25%
5         Obese    >31%    >25%
```

*Reference:

http://www.livestrong.com/article/102670-formula-calculate-body-fat-percentage/

http://www.calculator.net/body-fat-calculator.html


Example
===


A female in her 26 whose weight is 50Kg, and height is 170cm. 

Her body fat percentage and the description can be calculated by the following fuction.



```r
Result <- BodyFat(0, 50, 170, 26)
```

```
[1] "Body fat (%) =  21.3"
```

```
[1] "Description =  Fitness"
```
