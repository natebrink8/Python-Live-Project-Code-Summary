# Python Live Project
## Introduction
Two weeks of my Software Developer bootcamp at The Tech Academy were invested in developing a full-scale web site in Python, HTML, and CSS. The primary objective of my assigned stories of the project were to build CRUD functionality. 
The Python muscle I've been developing in the bootcamp was put to the test in the project's [back end stories](#back-end-stories) and I am proud to have completed these in short order. In addition, given much of the site framework had already been built, I made a significant HTML & CSS overhaul to the site's content in my [front end stories](#front-end-stories). Because I achieved the sprint's core assignments in 40% of the alloted time, I met with my Project Manager to discuss adding scope- namely expanding the database engagement and adding the functionality for the site to become a portal for fans of the four major sports in North America to interact.

Adding scope certainly accounted for an investment of time and challenges which were not on the the original project's radar but were excellent lessons to work through. Branching out also provided me the opportunity to work on other programming [skills](#other-skills-learned) that I'm confident I will use again on future projects.

Below are descriptions of the stories I worked on, along with code snippets and web site screenshots.

## Back End Stories
* [Build the basic App](#build-the-basic-app)
* [Create my model](#create-my-model)
* [Display all database items](#display-all-database-items)
* [Details page](#details-page)
* [Edit and Delete](#edit-and-delete)

### Build the basic App
The basic app creation contained HTML files for the base and index pages and the forms to use in the website.<br>
Home page (index):<br>
![Python Live Project: index page.](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/index-1.jpg)
<br>

### Create my model
The models.py file was initially built with a 'Fans' table to stand up the first instance of the site:<br><br>
![Python Live Project: Fans table class.](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/py-models-fans.jpg)<br>

The below views.py code was created for the Fans model, leveraging the FanForm from the forms.py and setting up for the "[Edit and Delete](#edit-and-delete)" functionality detailed below.<br><br>
![Python Live Project: Fans table view for create, update, and delete.](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/py-views_backend-2-and-5-create-update-delete.jpg)<br><br>


### Display all database items
The next step was to display all data being written to the database. The tallest task on this front was for all cities in Canada and the United States that have any of the four major professional sports teams. This maxes out with a city like New York, which has two teams in each of the four sports. The model for the ProCities table was built like this, in order to provide data points for all possible city needs:<br><br>
![Python Live Project: Model for the ProCities table .](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/py-models-cities.jpg)<br><br>

The views.py was built with four pieces defining:
1. the script for the import.
2. the link for the admin import page (using the script from step 1.)
3. the display of the table's details.
4. the Landing Page setup, to display the table's data.
<br>

![Python Live Project: views.py file for cities (1 of 2).](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/py-views_other-skills-6-cities-table-1.jpg)<br><br>
![Python Live Project: views.py file for cities (2 of 2).](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/py-views_other-skills-6-cities-table-2.jpg)<br>
(_each table required this same four piece construct but this example is solely for the 'ProCities' table_)<br>


### Details page
From the home page, a table's navbar item was built to be clicked to display its content:<br>
![Python Live Project: ProCities table display.](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/index-4-cities-display.jpg)<br><br>

Clicking a city name then drills down to the details page:<br>
![Python Live Project: ProCities table details.](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/index-4-cities-details.jpg)<br><br>


### Edit and Delete
(*Screenshot above details the code*: [Create my model](#create-my-model))<br>
The workflow for this is primarily for the Fans table, to be able to edit or delete a Fan record. Should the site progress for fans to interact and share reviews, etc, then login requirements would be added alongside the ability for a logged-in user to edit and delete their posts. For now, the site is built with edit and delete functionality for the Fans table:<br><br>
:sparkle:**Display**<br>
_Clicking a fan's name will display their record's details_.
![Python Live Project: Fans table display.](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/index-9-fans-display.jpg)<br><br>
**_View a fan record details_:**<br>
![Python Live Project: Fans table details.](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/index-9-fans-details.jpg)<br><br>
:sparkle:**Edit**<br>
![Python Live Project: Fans table update.](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/index-9-fans-update.jpg)<br><br>
:sparkle:**Delete**<br>
![Python Live Project: Fans table delete.](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/index-9-fans-delete.jpg)<br><br>


*Jump to: [Front End Stories](#front-end-stories), [Back End Stories](#back-end-stories), [Other Skills](#other-skills-learned), [Page Top](#live-project)*
<br><br>

## Front End Stories
### Page Format and Styling
* [Page Format and Styling](#page-format-and-styling)
The primary front end focuses were to frame out the necessary pages for the site I envisioned and then to pick the styling of my page and implement the HTML and CSS accordingly. Several templates were required to achieve the appropriate table interaction (see below.)<br><br>
![Python Live Project: list of Templates.](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/templates-list.jpg)<br><br>

The code for the Admin Import page was built to leverage the scripts in the views.py file (detailed in step 2 of the [Display all database items](#display-all-database-items) above):<br><br>
![Python Live Project: Admin Import page's code.](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/templates_admin-import.jpg)<br><br>

The code for the Cities display page was built with a "for each" loop to retrieve City and State names into the page:<br><br>
![Python Live Project: City display page's code.](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/templates_cities-display.jpg)<br><br>

The above then led to the following pages...<br><br>
1. the Admin Import page:<br><br>
![Python Live Project: Admin Import page.](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/index-12-admin-import.jpg)<br><br>

2. the City display page:<br><br>
![Python Live Project: Cities display page.](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/index-4-cities-display.jpg)<br><br>



*Jump to: [Front End Stories](#front-end-stories), [Back End Stories](#back-end-stories), [Other Skills](#other-skills-learned), [Page Top](#live-project)*
## Other Skills Learned
* CURIOSITY: Learning new efficiencies from other developers by observing their workflow and asking questions.
* COMMUNICATION: Improving project flow by communicating about who needs to check out which files for their current story.
* COLLABORATION: Practicing team programming when a bug is encountered but not solved (not spiraling).
* DISCOMFORT: Getting out of my comfort zone, taking responsibility for features out of the initial project scope, ensuring the structure of my site as well as the proper functionality, and loading symphonic data.
* PYTHON: Developing the Python grip! As a new developer, Python has been an exciting and fulfilling skill to add to my repertoire. Due to the nature of the site I wanted to create, I had extensive interaction with my models, views, and urls files. The site uses seven database tables (one for cities with professional teams, one for fans, and one for each of the four major sports.)
* OPERATIONS: I took the following steps to automate the Admin Import table loads:
    * CREATED the tables' infrastructure in the class.py file.
    * BUILT all of the CSV files for import. This was a major undertaking, given the breadth of the data sets being worked to the site.
    * LOADED the CSV files with all relevant data. The 'ProCities' table was the most extensive, with a row for every City/State/Country, as well as two columns for each major sport (to account for cities like New York, NY that have two teams in every major professional sport.) Here is the ProCities table, once loaded to the database:<br>
    ![Python Live Project: Cities display page.](https://github.com/natebrink8/Code-Summary/blob/main/README-screenshots/database-1-ProCities.jpg)<br>
    * CREATED the import scripts in the views.py file.
    * CONSTRUCTED an Admin Import page with buttons hyperlinked to execute the import scripts.
    * RAN all of the import scripts, troubleshooting data corruption issues.
        * There was a particular roadblock in the Admin Import page (an added feature) so I worked with my Project Manager to vet the troubleshooting I'd performed on the code. As we viewed the errors, I identified foreign characters which were not within the code but that Excel introduced within the CSV file. Given my experience with large sets of data, I cleaned up the data in Notepad++, renamed the old Excel CSV, then saved the new comma-separated text file with the name my program was seeking and corrected the failed import. This was found to be the case in all six tables I was loading in the database. I created and shared a set of steps for future developers to take to resolve data corruption issues on large sets of data, to use Extended and Regular Expression searches.
    * COPIED the CSV files in the root directory and pasted them there.
    * RENAMED the CSV import files, adding "-loaded" to the new file names.
    * MOVED the "-loaded" CSV files to an Archive subfolder.
    * CLEARED the data from the root directory CSV files, leaving just the column headers (preventing potential accidental import / overwrite of the database.)
<br><br>
  
*Jump to: [Front End Stories](#front-end-stories), [Back End Stories](#back-end-stories), [Other Skills](#other-skills-learned), [Page Top](#live-project)*
