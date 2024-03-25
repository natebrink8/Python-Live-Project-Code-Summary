# Live Project
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
The basic app creation contained HTML files for the base and index pages and the forms to use in the website:
    screenshot 1

### Create my model
[ADD description and code snippet here]
    screenshot 2-and-5

### Display all database items
[ADD description and code snippet here]

### Details page
[ADD description and code snippet here]

### Edit and Delete
[ADD description and code snippet here]
    screenshot 2-and-5


*Jump to: [Front End Stories](#front-end-stories), [Back End Stories](#back-end-stories), [Other Skills](#other-skills-learned), [Page Top](#live-project)*
## Front End Stories
* [Front End Improvements](#front-end-improvements)
* [Page Format and Styling](#page-format-and-styling)

### Front End Improvements
[ADD description and code snippet here]
### Page Format and Styling
[DETAIL work done on formatting in CSS and screenshots]


*Jump to: [Front End Stories](#front-end-stories), [Back End Stories](#back-end-stories), [Other Skills](#other-skills-learned), [Page Top](#live-project)*
## Other Skills Learned
* CURIOSITY: Learning new efficiencies from other developers by observing their workflow and asking questions.
* COMMUNICATION: Improving project flow by communicating about who needs to check out which files for their current story.
* COLLABORATION: Practicing team programming when a bug is encountered but not solved (not spiraling).
* DISCOMFORT: Getting out of my comfort zone, taking responsibility for features out of the initial project scope, ensuring the structure of my site as well as the proper functionality, and loading symphonic data.
* PYTHON: Developing the Python grip! As a new developer, Python has been an exciting and fulfilling skill to add to my repertoire. Due to the nature of the site I wanted to create, I had extensive interaction with my models, views, and urls files. The site uses seven database tables (one for cities with professional teams, one for fans, and one for each of the four major sports.) I took the following steps to automate the table loads:
    * CREATED the tables' infrastructure in the class.py file.
    * BUILT all of the CSV files for import.
    * LOADED the CSV files with all relevant data. The 'ProCities' table was the most extensive, with a row for every City/State/Country, as well as two columns for each major sport (to account for cities like New York, NY that have two teams in every major professional sport.)
    * CREATED the import scripts in the views.py file.
    * CONSTRUCTED an Admin Import page with buttons hyperlinked to execute the import scripts.
    * RAN all of the import scripts, troubleshooting data corruption issues.
        * There was a particular roadblock in the Admin Import page (an added feature) so I worked with my Project Manager to vet the troubleshooting I'd performed on the code. As we viewed the errors, I identified foreign characters which were not within the code but that Excel introduced within the CSV file. Given my experience with large sets of data, I cleaned up the data in Notepad++, renamed the old Excel CSV, then saved the new comma-separated text file with the name my program was seeking and corrected the failed import. This was found to be the case in all six tables I was loading in the database. I created and shared a set of steps for future developers to take to resolve data corruption issues on large sets of data, to use Extended and Regular Expression searches.
    * COPIED the CSV files in the root directory and pasted them there.
    * RENAMED the CSV import files, adding "-loaded" to the new file names.
    * MOVED the "-loaded" CSV files to an Archive subfolder.
    * CLEARED the data from the root directory CSV files, leaving just the column headers (preventing potential accidental import / overwrite of the database.)
* OTHER SKILL 3.
  
*Jump to: [Front End Stories](#front-end-stories), [Back End Stories](#back-end-stories), [Other Skills](#other-skills-learned), [Page Top](#live-project)*