# Flight Deal Finder

This is a Python program that searches for the lowest prices of flights from a given origin city (LON in this case) to various destinations listed in a Google Sheet. If a lower price is found than the current listed price on the Google Sheet, a SMS alert is sent to the user.   

# Installation

To run this program locally, you will need to install the required packages in your environment.   

You need to set up environment variables for your own APIs.  

The program uses the following APIs:

~~~
Sheety API - for the Google Sheet integration
Twilio API - for the SMS alert
Tequila Flight Search API - for the flight search
~~~
  
Prerequisites:  
~~~
Python 3.x
Sheety account
Twilio account
Tequila account
~~~

![Flight Deal Finder](https://github.com/filosoho/Flight-Deal-Finder/blob/34e345ee882dae3977b6bd2ac9f906fea3f83748/1.jpg) 




# Features

* Queries Google Sheets API to get destination data including city name and IATA code.
* Queries the Flight Search API to check flights for the next 6 months and return the lowest-priced flights.
* Sends SMS notifications with the deal flight details, including origin and destination airports, departure and return dates, and ticket price.

# How to use

Run the program using:
~~~
main.py
~~~

The program will query the Google Sheets API to get the destination data and check flights for each destination over the next 6 months. If a flight is found with a price lower than the lowest price listed in the Google Sheet, the program will send an SMS notification with the deal flight details.  

<br>

If you want to test the script without actually sending an SMS, uncomment the print statement in the code.

# Contributing
If you would like to contribute to this program, feel free to submit a pull request. Please include a detailed description of the changes made and the reasons for the changes.

# License
Feel free to use and modify the code as per your requirements. 
