# Amazon-Price-Tag-Selenium
It's a code to scrape through amazon webpage and access the data of a particular user specified product and get hold of the price tag and send the details to the user through sms using twilio.
Explanation:-
1. get_amazon_product_price: This function uses Selenium to open the provided Amazon product URL, find the element that contains the price (you may need to adjust the find_element_by_id or other locator method based on Amazon's HTML structure), and return the price as text.
2. send_sms: This function initializes a Twilio client using your Twilio account SID and authentication token. It then sends an SMS message to the specified to_number with the provided message.
3. Main program:
     >Asks the user for an Amazon product URL.
     >Uses get_amazon_product_price to fetch the price.
     >If the price is successfully fetched, it constructs a message and sends it using send_sms.
     >Prints success or failure messages accordingly.
Notes:-
     >Make sure to replace "your_account_sid", "your_auth_token", "your_twilio_phone_number", and "your_phone_number_to_receive_message" 
      with your actual Twilio credentials and phone numbers.
     >Adjust the find_element_by_id method or other locator methods in get_amazon_product_price based on the specific HTML structure of the 
      Amazon product page you are scraping.
     >Handle exceptions and edge cases (like product not found) as per your application's requirements.

This script should enable you to scrape the price of a product from Amazon and send it as an SMS using Twilio.
