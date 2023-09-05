## General Assembly TOP Program for CFPB

# Table of Contents:
- Background
- Introduction
- Research
- Problem Statement
- Data Dictionary
- Brief Summary of Analysis
- Conclusions and Recommendations
- File Structure
- Sources

## Data Dictionary
|Feature|Type|Description|
|:---|:---:|:---:|
|**Agreement_Date**|*datetime*|6-month interval for a given year when this report was provided by participants|
|**Institution_Name**|*object*|The name of the Institution that issued the credit card plan.|
|**Plan_Name**|*object*|The name of the credit card plan.|
|**Availability_of_Credit_Card_Plan**|*object*|States whether the credit card is available nationally, regionally, or only in one state. Options include: National, Regional, and One State.|
|**Location**|*object*|If the credit card plan is available regionally or within a single state, the ‘Location’ column will list the state(s) in which the credit card plan is available. In the event the credit card plan is available nationally, the ‘Location’ cell will be null.|
|**APR**|*float64*|“Annual Percentage Rate” states the annualized interest rate that is used to compute finance charges for purchases. If the purchase APR for new customers varies by customer segment, the APR reported is the midpoint of the range of APRs offered to new customers of the product as of the reporting date.|
|**Index**|*object*|Displays V (variable) in the event the credit card plan’s interest rate is variable. If the credit card plan has a fixed interest rate, then the Index column will display F (fixed).|
|**Variable_Rate_Index**|*object*|If the credit card plan has a variable rate, the ’Variable Rate Index’ column shows the index used to set the rate. Options include: Prime, One-month T-bill, Three-month T-bill, Six-month T- bill, One-year T-bill, Fed Funds, Cost of Funds, Federal Reserve Discount Rate, and Other.|
|**Grace_Period**|*float64*|States the period of time from the end of the billing cycle in which credit extended for purchases during that billing cycle may be repaid without incurring a finance charge.|
|**Annual_Fee**|*float64*|Changed from "Annual Fee" for processing. The annual charge, expressed as an annualized amount, that is imposed for the issuance or availability of the credit card.|
|**Late_Fee**|*float64*|The fee imposed by an issuer for a late payment.|
|**Telephone_Number_for_Consumers**|*object*|The phone number where the institution in question can be reached.|

Sources:
1. CFPB Credit Card Plan Survey: https://cfpb.my.salesforce-sites.com/CreditCardPlanSurveys
2. CFPB Credit Card Plan Reference Guide: https://cfpb.my.salesforce-sites.com/CreditCardPlanSurveys/resource/1600984878000/TccpPublicSiteQuickReferenceGuide (Page 4)
3. CFPB Credit Card Late Fees Report: https://s3.amazonaws.com/files.consumerfinance.gov/f/documents/cfpb_credit-card-late-fees_report_2022-03.pdf