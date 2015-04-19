---
title       : Loan Repayment App
subtitle    : Course Project - Developing Data Products
author      : 
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme: solarized_light
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---   

## Planning to buy something expensive?

- Thinking of buying something expensive like a car or a house?  
- But do not have enough money to pay upfront  
- You probably will look at getting a loan  
- [Loan Repayment Application](https://bmat.shinyapps.io/LoanRepayment/) provides a simple way to find some of the information that you need to make you decision 

--- .class #id 

## A simple and easy way to work out details of the loan

- [Loan Repayment Application](https://bmat.shinyapps.io/LoanRepayment/) is a very simple tool to work out the details of loan that you might want to borow  
- It allows you to play around with the key variables in borrowing
- And provide you the information on the contribution of you payment towards interest and the loan principal amount
- <span class = 'red'>Note: </span> Do consult your lender of other options they may have before finalising you decision


--- &twocol w1:50% w2:50%

## Check out the charts ...  

- Charts showing proportion towards interest and principal for 30 and 20 year loans
- The area in red shows the proportion that you pay towards interest; Longer the loan term, higher the proportion that goes to interest.

*** =left

![plot of chunk unnamed-chunk-1](assets/fig/unnamed-chunk-1-1.png) 


*** =right

![plot of chunk unnamed-chunk-2](assets/fig/unnamed-chunk-2-1.png) 


---

## ... and the table with the breakdown   

   

```r
library(xtable)
print(xtable(paymentBreakDown[1:3,]), type="html") #display first few lines
```

<!-- html table generated in R 3.1.2 by xtable 1.7-4 package -->
<!-- Sun Apr 19 00:57:54 2015 -->
<table border=1>
<tr> <th>  </th> <th> year </th> <th> period </th> <th> repayment </th> <th> toPrincipal </th> <th> percentToPrincipal </th> <th> remainingPrincipal </th>  </tr>
  <tr> <td align="right"> 1 </td> <td> 1 </td> <td> 1 </td> <td align="right"> 1254.66 </td> <td align="right"> 254.66 </td> <td align="right"> 20.30 </td> <td align="right"> 149745.34 </td> </tr>
  <tr> <td align="right"> 2 </td> <td> 1 </td> <td> 2 </td> <td align="right"> 1254.66 </td> <td align="right"> 256.36 </td> <td align="right"> 20.43 </td> <td align="right"> 149488.98 </td> </tr>
  <tr> <td align="right"> 3 </td> <td> 1 </td> <td> 3 </td> <td align="right"> 1254.66 </td> <td align="right"> 258.07 </td> <td align="right"> 20.57 </td> <td align="right"> 149230.91 </td> </tr>
   </table>
  

```r
print(xtable(paymentBreakDown[238:240, ]), type="html") #display last few lines
```

<!-- html table generated in R 3.1.2 by xtable 1.7-4 package -->
<!-- Sun Apr 19 10:56:40 2015 -->
<table border=1>
<tr> <th>  </th> <th> year </th> <th> period </th> <th> repayment </th> <th> toPrincipal </th> <th> percentToPrincipal </th> <th> remainingPrincipal </th>  </tr>
  <tr> <td align="right"> 238 </td> <td> 20 </td> <td> 238 </td> <td align="right"> 1254.66 </td> <td align="right"> 1229.90 </td> <td align="right"> 98.03 </td> <td align="right"> 2484.48 </td> </tr>
  <tr> <td align="right"> 239 </td> <td> 20 </td> <td> 239 </td> <td align="right"> 1254.66 </td> <td align="right"> 1238.10 </td> <td align="right"> 98.68 </td> <td align="right"> 1246.38 </td> </tr>
  <tr> <td align="right"> 240 </td> <td> 20 </td> <td> 240 </td> <td align="right"> 1254.69 </td> <td align="right"> 1246.35 </td> <td align="right"> 99.34 </td> <td align="right"> 0.00 </td> </tr>
   </table>




