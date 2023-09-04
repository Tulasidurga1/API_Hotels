# API_Hotels
# Hosted Link:-https://tulasidurga1.github.io/API_Hotels/
### HTML Structure:
The HTML file begins with a standard document type declaration (<!DOCTYPE html>) and sets the document's language to English.
Inside the <head> section, there are meta tags for character set and viewport settings, a title for the page ("Hotel Search"), and a link to an external CSS file named "style.css."
The <body> section contains the main content of the page.
### Header:
- There's a <header> element containing an <h1> with the title "Hotel Search."
# Search Form:
- A <div> with a class of "input" contains the search form elements.
- There are three input elements:
- One for entering the destination ("Going to").
- One for selecting the dates.
- One <select> element for choosing the number of travelers (adults or children).
- There is also a "Search" button with the class "src."
### Card Container:
A <div> with the id "cardContainer" is provided. This is where the search results will be displayed.
# JavaScript:
- In the JavaScript section, several variables are declared and initialized. These variables include response, jsonData, url, and options, which are used to fetch data from a remote API related to hotel information.

- There is a try-catch block for fetching data from the API using the Fetch API. If the fetch is successful, the response is converted to JSON, and the resulting data is logged to the console. If there's an error, it is also logged.

- The jsonData variable is used to store the retrieved data from the API.

- Several HTML elements are selected using their IDs and stored in variables, including area, date, button, and cardContainer.

- There is a function named filterDataByName(name) that filters the data based on the entered destination name (country code in this case). It checks if the name is empty and, if not, filters the data to find matching countries by their country codes.

- Another function named displayFilteredData(filteredData) is defined to display the filtered data as hotel cards in the "cardContainer."

- An event listener is attached to the "Search" button (button) to handle the search functionality. When the button is clicked, it prevents the default form submission, gets the value from the destination input (area), and the date input (date), and then filters and displays the matching data.

- Finally, the displayFilteredData(jsonData) function is called to initially display all the data when the page loads.
