---
layout: post
title: COMM 121 Intro to Finance --- Note 2: About APR, EAR, Compounding Frequency, Payment Frequency, and Discount Rate
tags:  post 2
categories: demo
---


## About APR, EAR, Compounding Frequency, Payment Frequency, and Discount Rate

- APR: Annual Percentage Rate, also known as quoted annual interest rate, simple annual interest rate. Annual interest rate without consideration of compounding. 
APR is meaningful only if the compounding frequency within a year is given. 

- EAR: Effective Annual Interest Rate. Annual interest rate after taking compounding into account. 
EAR is meaningful without a compounding frequency because we must go through the math of compounding frequency to get this rate. We can call it ex-post interest rate
to some extent. 

- Compounding Frequency: the number of periods that "the money that money makes"(accumulated interest) and the principal make money for you during certain time interval. Usually, this time interval is a year. 
Typical compounding frequency: Year, Semi-Annual, Quarterly, Monthly, Bi-Weekly, Weekly, Daily, and continuous compounding(the compounding frequency goes to the infinity).

Suppose APR is r, and compounding frequency is m, think aobut the formula to convert APR to EAR: (1+r/m)^m = 1+EAR
Since the limit of (1+r/m)^m when m goes to the infinity is e^r, we have an upper bound of EAR for an APR compounded m times over a year. For example, an APR of 10% 
compounded quarterly, the EAR would be 10.38129%. If compounded daily, the EAR would be 10.51558%. The EAR is increasing as the compounded frequency goes up, and the EAR converges to 10.52% (e^.1) if compounded continuously. We see the largest difference between APR and EAR is 52 basis points here. As APR increases, the largest gap between APR and EAR is widder, think about the graph of e^x. You can try APR=0.3 and APR=0.5 and find their EARs for exercise. 

- Payment Frequency: the number of times when a borrower makes interest payment. You can also think about it as the time interval between each cash flow. 
- Discount rate: the effective interest rate that a borrower pays interest for a period of time. Discount rate must match with payment frequency. 

`Important comments about the above notions:`

1. EAR equals APR when compounded annually. 
2. An effective interest rate for a certain time interval equals simple interest for that period when APR is quoted as compouned at the same 
frequency as the payment frequency. For example, An APR of 7% compounded monthly, the simple monthly interest rate is 7%/12=0.0058333...While the EAR is (1+7%/12)^12-1=0.072290081, and the effetive monthly interest rate is (1+EAR)^(1/12)-1, which is exactly 0.0058333...If you think about the math here, ((1+APR/m)^m-1+1)^(1/m)-1=APR/m. 

However, if APR is quoted as compounded at a different frequency than the payment frequency. The effective interest rate for the payment interval is different
than the simple interest rate for the same time interval. To see this, think about the above example again. An APR quated as compounded m times a year but the payment
is made n times a year. We have an EAR that equals (1+APR/m)^m-1, and the effective interest rate for the payment period is ((1+APR/m)^m-1+1)^(1/n)-1, which does not equal APR/m. 

This is the case where how Canadian banks quote mortgate rate. They usually quote APR as compouneded semi-annually, but a borrower makes mortgage payment monthly. We 
need to work out the effective monthly interest rate to get the monthly payment number. See example 5.24 on page 121 for detail. 


