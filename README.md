# SSRS-Report-of-Dow-Jones-Components
Shows charts and information about the 30 stocks in the Dow Jones

Here's what part of one of the reports looks like:
![](https://github.com/ovnisoftware/SSRS-Report-of-Dow-Jones-Components/blob/master/SSRSReport.jpg)

How to get this SSRS report to work:

1. Setup your database on SQL Server that holds the stock information.  Two options here:

 1A. Restore the DJIAComponents.bak file I included in this repo (DJIAComponents.bak has 1 table with stock quote information of the 30 components of the Dow Jones Industrial Average from 1/2/15-4/24/15)

 or...

 1B. Pull down new quotes using this app I built:

 https://github.com/ovnisoftware/YahooFinanceQuoteDownloader

 and then you can bulk insert the .csv stock data you pull down into SQL with this script I also wrote:

 https://github.com/ovnisoftware/Bulk-Import-CSV-Stock-Quotes-Into-SQL-Server-Script

2. Update the connection strings in the SSRS project in Visual Studio 2013 to connect to whatever database table you just setup.

3. Run the SSRS reports.
