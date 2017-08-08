# Business Tax Report

Suitable for periodic business activity reporting within Gnucash

# Installation
* _config.user_ illustrates modification to existing file in ~/.gnucash folder
* _business-tax-report.scm_ could be copied to ~/.gnucash/report folder

# Instructions
You will need to set up tax holding accounts, usually liability or asset accounts, which will hold splits in multisplit transactions.
You must record these accounts using Business > Tax Tables as described. An example of multisplit transaction is as follows:
* Income:Sales -$100
* Liability:SalesTaxHolding -$10
* Asset:Bank $110

To run report, run Report > Collected Reports > Business Tax Report, and select Income & Expense business accounts in the Accounts tab.

Example report: http://htmlpreview.github.io/?https://raw.githubusercontent.com/christopherlam/bas-report/master/bas1.html 
and http://htmlpreview.github.io/?https://raw.githubusercontent.com/christopherlam/bas-report/master/bas2.html

To submit suggestions, bugs etc please send feedback in github.
