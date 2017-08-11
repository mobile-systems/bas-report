# Business Tax Report

Suitable for periodic business activity reporting within Gnucash

# Installation
* _config.user_ illustrates modification to existing file in ~/.gnucash folder
* _business-tax-report.scm_ could be copied to ~/.gnucash/report folder

# Instructions
You will need to set up tax holding accounts, usually liability or asset accounts, which will hold splits in multisplit transactions.
You must record these accounts using Business > Tax Tables as described. An example of multisplit transaction is as follows:
* Income:Sales -Rs 100
* Liabilities:GST:CGST:Output CGST -Rs 9
* Liabilities:GST:CGST:Output SGST -Rs 9
* Asset:Bank Rs 118

The Tax Table names which are supported (and need to be created separately for each gnucash file) are given in a image file, includes 
* "Input"
* "Input 5" 
* "Input 5 InterSt"
* "Output"
* "Output 5"
* "Output 5 InterSt"
(InterSt stands for InterState)
etc to account for the tax slabs 0%, 5%, 12%, 18%, 28%.

To run report, run Report > Collected Reports > Business Tax Report, and select Income & Expense business accounts in the Accounts tab.

The final report and the tax liability column doesn't take into considerations the rules for setoff of IGST Input Credit, and one has to
do the calculation in a spreadsheet format that has been added here.

Example report: http://htmlpreview.github.io/?https://raw.githubusercontent.com/christopherlam/bas-report/master/bas1.html 
and http://htmlpreview.github.io/?https://raw.githubusercontent.com/christopherlam/bas-report/master/bas2.html

To submit suggestions, bugs etc please send feedback in github.

