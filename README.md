
# Create react App
**Create a react app called stocks.**

# StockTracker

Create in JSON format a file containing information on financial stocks from 5 companies. 

Each stock has metadata associated with it.

 Your goal is to output that data from an external file and render it on the web page in a table format, as shown below.



# Add JSON Data to a File

 Create a js file in your project inside your src folder. Called data. It should be src/data.js. Inside that file you should format the information for each company in as a JSON. 

 name the array of the JSON stockData. Each JSON object inside the array should contain the following information: 

- Name of the company
- Stock ticker for the company
- Price of its stock



# Update App Component

Open your App.js file and remove the boilerplate code that is in between the div tags. 

# Create Stocks Component

Now create a new component called Stocks.js inside your src folder. 
src/Stocks.js 

Return an h1 tag that says "Welcome to the Stock Tracker" with a class name of stock-container.

import App.css to this component. 

Add the following code to App.css: 
.App {
  text-align: center;
}

.stock-container {
  padding-left: 3em;
  padding-right: 3em;
  margin-top: 3em;
}

.

Head back to your App.js file and import your Stocks.js component and render the component to show on your webpage. 


# Load JSON Data into Stocks Component

Get the JSON data from the src/data.js file and render it inside <Stocks>.  Add this import in your src/Stocks.js file.


Next iterate over the stockData array imported from the data.js file. Inside your <Stocks> component, add the logic to go over every element from the stockData array using .map function().



# Display Stock Information In a Table Format

Add a <HomePageHeader> component to display a header.

Add a h2 tag titled "Yor Stock tracker" Give the h1 tag a className of header. 

add this code to App.css
.header {
  background-color: #f4e04d;
  min-height: 10vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  font-size: calc(10px + 2vmin);
  color: #10375c;
}


Create a Stock component. 

The <Stock> component will accept data in props and render a table on the web page. You will need to use props to add information to the table format. 

This component accepts props and returns an HTML table for a stock with four columns rendering the company name, ticker, stock price, and time elapsed in seconds.

Next do some styling in App.css that will look similar the image above. 


Finally, refactor the <Stocks> component so it can call the <HomePageHeader> and <Stock> components we just created. 

The code should render the <Stocks> component containing a <HomePageHeader> and <Stock> for every element in inside the stockData array. Instead of displaying the JSON data inside a div, you'll now pass it as props to <Stock> component.