# UFOs
 unit 11
UFOs
For learning Java Script from Module 11

Project Overview
Dana wants build a webpage with dynamic table to provide a more in-depth analysis of UFO sightings by allowing users to filter for multiple criteria at the same time. Table filters dana considers are for the date, city, state, country, and shape

Resources
javascript, HTML, Bootstrap, Visual Code, Browser Edge
data for table from data.js, index.html
Challenge Overview
Prerequisite:

Download the ufo_starterCode.ipynb file
Deliverable 1: Filter UFO sightings on multiple criteria
Follow the instructions below and the numbered comments in the starter code to complete Deliverable 1.

Download the ufo_starterCode.js, rename it app.js, and place it in the js folder of your UFOs GitHub repository. The starter code includes the code used to populate the table from this module.
In the index.html file, remove the list (
) element that creates the button.
Create four more list elements: city, state, country, and shape. These will be similar to the "Enter Date" list element. Each element should have the same "id" as the object properties in the data.js file.
In the app.js file, create an empty filters variable to keep track of all the elements that change when a search is entered. This variable will be used in Step
5 to store the property “id” and the value that was entered from user input.
Next, you will need to write code for two functions whose names we’ve provided in the starter code, updateFilters() and filterTable().
The updateFilters() function will replace your handleClick() function and update the filters variable you created in Step 1.
The filterTable() function will filter the table data by the value that is entered for the "id" that has changed.
At the end of the starter code (located before the buildTable(tableData) function), modify the event listener from this module so that it detects a "change" on each input element and calls the updateFilters() function.
Inside updateFilters function, you’ll write code in Steps 4-5 to update the filters based on user input.
Create a variable that saves the element that was changed using d3.select(this).
Create a variable that saves the value of the changed element’s property.
Create a variable that saves the attribute of the changed element’s id.
Write an if-else statement that checks if a value was changed by the user (variable from Step 11). If a value was changed, add the element’s id (variable from Step 12) as the property and the value that was changed to the filters variable you created in Step 1. If a value was not entered, then clear the element id from the filters variable.
Inside the updateFilters() function, call the filterTable() function that will be used in Step 15.
In the filterTable() function, write code to filter the table based on the user input that is stored in the filters variable.
Create a variable for the filtered data that is equal to the data that builds the table. This variable will hold the updated table data based on the user input.
Loop through the filters object and store the data that matches the filter values in the variable created in Step 15.
Rebuild the table with the filtered data by passing the variable created in Step 15.
UFO sightings-Analysis Results
UFO sightings initial load image_name

UFO sightings with Date filter

Enter a date and press enter.
The table data will be filtered on that date. image_name
UFO sightings with Date and state filter

Enter a date and state code and press enter.
The table data will be filtered on that date and state. image_name
UFO sightings with Date,State and Shape filter

Enter a date,state code and shape press enter.
The table data will be filtered on that date,state and shape. image_name
UFO sightings with Date,State,Shape and City filter

Enter a date,state code, shape and city press enter.
The table data will be filtered on that date,state, shape and city. image_name
UFO sightings with country filter

Enter a country code press enter.
The table data will be filtered on that country. image_name
UFO sightings-Analysis Summary
Drawbacks:

We have limited data available with data from countries like US and Canada only.
The UFO sightings are pretty old and from the year 2010, that too from first 13 days only.
There is no clear button to clear the search.
The search is done by one at a time.
Additional recommendations:

We could have added a chart also for better presentation.
instead of type in the values, we could have added a drop down and select from the list.
