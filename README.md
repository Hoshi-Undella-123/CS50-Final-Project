# CS50-Final-Project

# PANDEMIC METRICS
#### Video Demo: <https://youtu.be/lbbDS20nlj8>
#### Description:

```
Hello, my name is Hoshita Undella, and for my cs50 project I designed a web-based application using primarily Python and Flask for the backend and HTML/CSS/JS and jQuery for the UI. My project focuses on providing everyone with user-friendly access to accurate information regarding Covid-19. I did my project using PyCharm IDE instead of CS50 because I felt more comfortable using that IDE for complex projects. My project has two modules both of which reside in my main project file called “cs50prj”.
```
```
My first module is to capture data into a database. The information being captured is state, country, city, facility, number of patients admitted, and number of patients recovered.  I entered dummy data into the database.
```
```
For this, I created a rest API, which is located in the file called “rest_server.py”. The API is “api/v1/resources/facilities/add” which helps ingest the data captured from UI into the database. I also created the “db_manager.py” library to verify the validity of data at server before handing it over to the “db_library.py”.
```
```
Lastly, to capture new patient’s data into the database from UI, I created the insert function of “db_util.py” library, which is called under the “api_add_record” function in “rest_server.py”. I also created a user-friendly “patients.html” page with text boxes and buttons to submit data for new patients and facilities into the database.
```
```
For my second module, I displayed the data that was captured using the first module. I have created “facilities.html” to display a table with all of the corresponding information such as state, county, city, facility, number of patients admitted, patients recovered, and patient deaths along with a search box.
```
```
The second API is “api/v1/resources/facilities/all” through which data from around the nation can be retrieved from the database. The third API used is a State Specific API (api/v1/resources/facilities/<state>) that returns information based upon the state specified. I also created the “manage_data.py” library with multiple functions to prepare data for the UI, which was returned by the “db_util.py” library.
```
```
Lastly, in order to make my web application even more user friendly, I created a search function on UI,  which implements a search criteria. Using this, the user can type any information regarding Covid-19 such as a facility name and the search tool will narrow down the display to only the corresponding data rows
```
```
I implemented all the REST API’s using the Flask framework.
```
```
Overall, the objective of my project was to create an effective tracking system with Covid-19 patient data from around the Country in order to bring awareness and essential information to all people. Because my project is open source and has UI friendly features such as a search bar, it is easily accessible, which allows for accurate representation of facilities for effective admission of Covid-19 infected patients so that they can receive immediate care.
```
