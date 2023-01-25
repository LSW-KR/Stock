Create_List_Error
>This code is written in Python and is used to scrape stock market data.
>This code is a test code to check for stock code.

>> 1. First, it imports the 'pykrx' library which is a python wrapper for the Korea Exchange (KRX) website. This library is used to scrape data from KRX.
>> 2. It also imports the 'pandas' library which is used to manipulate and analyze data.
>> 3. The 'FinanceDataReader' library is also imported, which is used to access the financial data of various markets.
>> 4. It then imports 'datetime' library that is used to handle date and time.
>> 5. 'mariadb' library is also imported which is a python wrapper for MariaDB, it is a relational database management system.
>> 6. It then creates an empty DataFrame and assigns 'stock' attribute to it.
>> 7. It then uses the 'StockListing' function from the 'FinanceDataReader' library to retrieve a list of stocks listed on the KOSPI and KOSDAQ markets.
>> 8. It then appends the KOSDAQ stock data to the KOSPI stock data.
>> 9. It then creates a list of symbols of the stock and assigns it to the variable 'symbol_list'.
>> 10. The last line of the code prints the last item in the symbol_list.

>Note: This script uses the 'FinanceDataReader' library to access the financial data of various markets. Users need to install this library before running this script. 
It is also important to note that this script is only importing the libraries, creating a DataFrame and retrieve the stock symbols of the KOSPI and KOSDAQ markets. Any further functionality would need to be added to the script in order to utilize the data.


Stock_List
> 1. This is Python code used for scraping historical stock market data, storing it in a MariaDB database, and sending notifications through Telegram when certain conditions are met.
> 2. The code uses several libraries, including pykrx, pandas, FinanceDataReader, and telepot, to accomplish its tasks.
> 3. The pykrx library is used to scrape historical stock market data from the KRX (Korea Exchange) website. The FinanceDataReader library is used to retrieve the list of symbols for the KOSPI and KOSDAQ stock markets.
> 4. The pandas library is used to manipulate the data and store it in a DataFrame. Then, the mariadb library is used to connect to a MariaDB database and insert the data into a table called "stock_daily".
> 5. The telepot library is used to interact with the Telegram API to send notifications. The code uses the telepot.Bot class to create a Telegram bot and the getMe() method to retrieve information about the bot.
> 6. The code also defines several functions to handle different tasks, such as connecting to the database, creating an SQL statement to insert the data, and sending notifications through Telegram.
> 7. The main() function is the entry point of the script where it starts to iterate over the symbol_list, retrieve the data, manipulate it, store it to the database, and sending notifications if the Open value of the stock is exist or blocked.
> 8. This script is designed to be run periodically (e.g. daily) to update the database with new stock market data.
