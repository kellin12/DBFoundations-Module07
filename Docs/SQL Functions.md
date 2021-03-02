# SQL Functions
**Dev:** *Kelli Nakamura*

**Date:** *02-28-2021*

## Introduction
In this paper, I will be explaining when to use a SQL user-defined function and the differences between scalar, inline, and multi-statement functions.

## SQL User-Defined Functions
SQL User-Defined Functions (UDFs) are custom functions that the user develops for their database. Similar to built-in functions, you can program these functions and call on them as many times as needed. To optimize the use of a UDF, it is recommended to create and use a UDF when it involves calculations, especially involving a complex script. Additionally, like views, you can create the UDF when you expect to frequently call on the function. For example, a manager may want to review inventory count KPIs monthly. The KPIs require a calculation comparing the monthly counts. The user can create a UDF for these KPIs since it involves a calculation (Figure 1). Additionally, creating the UDF will provide efficiency since the manager would like to review the KPIs monthly. The user can call the UDF, rather than rewrite the script every month. 

![alt text](https://github.com/kellin12/DBFoundations-Module07/blob/main/Docs/KPI%20Script%20Screenshot.png "Figure 1: Example of a function created for inventory count KPIs")
Figure 1: Example of a function created for inventory count KPIs

## Scalar, Inline, and Multi-Statement Functions
There are three types of user-defined functions: scalar, inline, and multi-statement. A scalar function returns a single value as an expression. An inline function returns a table as a result of the actions performed by the function and is derived from a single Select statement. Multi-statement functions return a table of data, like an inline function, but can be derived from multiple SQL statements. 

## Summary
In summary, UDFs are another option to provide efficiency when extracting data from a database. Depending on the data needed, a scalar, inline, or multi-statement function will be created and used. 
