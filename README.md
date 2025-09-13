# Amazon Product Web Scraper & Price Tracker
This project is an automated web scraper built in Python to track the price of a specific product on Amazon. It scrapes the product's title, price, and customer ratings, stores the data over time, and includes a function to send an email notification if the price drops.

## Features
- Web Scraping: Uses the requests and BeautifulSoup libraries to scrape a product's title, price, and customer ratings from an Amazon product page.

- Data Storage: The scraped data, along with the date, is saved to a CSV file (Web Scraper.csv).

- Price Tracking Automation: A function price_check() is defined to perform the scraping and data saving. It is set to run automatically every 24 hours using a while loop and time.sleep().

- Email Notification: Includes a send_mail() function using the smtplib library to send an email alert when the price of the item is low.

## Requirements
To run this script, you will need the following Python libraries installed:
- requests
- beautifulsoup4 (bs4)
- pandas
- smtplib (standard library)
- datetime (standard library)

## Output
<img width="647" height="187" alt="Screenshot 2025-09-12 at 10 31 17 PM" src="https://github.com/user-attachments/assets/5ca2f00d-8515-43bc-a9c8-77fee70c9a49" />


## Usage
- Clone the Repository: Clone this repository to your local machine.

- Update the URL: Modify the URL variable in the script to the Amazon product page you wish to track.

- Set up Headers: Add your user-agent to the headers variable to avoid being blocked by Amazon.

- Configure Email: In the send_mail() function, update the sender's email and the app-specific password to your own credentials.

- Run the Script: Execute the Jupyter Notebook cells to start the web scraper and price tracker. The script will automatically scrape the data daily and append it to the CSV file.

## Author
**Samridh Rastogi** - https://github.com/Samridh27
