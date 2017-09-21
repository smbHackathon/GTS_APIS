# GTS APIs
## Description for GTS Sanbox
Global Trade Solution(GTS) enables users to calculate import duty and taxes in a few quick steps, when you are importing goods into the USA, EU, Russia, Canada and many more countries. Along with Duty & Taxes, GTS also returns if there is any applicable restriction.

# Duty Calculator
```
API URL:                http://www.dutycalculator.com/api2.1/sandbox/
API key for Sandbox:    2bac6dba1354599a
Reference document:     https://docs.google.com/document/d/1_C5XqlAOlw_jv62idHev5Dpu6z6clxFk9l4q_M_OAvs/pub 
```
Note: This is a sandbox account. All the API validations will be done however the response for any request will be static.</b>

```
For Instance, 

http://www.dutycalculator.com/api2.1/sandbox/2bac6dba1354599a/get-hscode?from=usa&to=ind&desc[0]=waterBottle&detailed_result=1

Will provide the same response as of

http://www.dutycalculator.com/api2.1/sandbox/2bac6dba1354599a/get-hscode?from=usa&to=ind&desc[0]=iphone&detailed_result=1
```
