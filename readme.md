# Test task

Do manual testing of provided application, find bugs and provide suggestions for UI/UX.

## Expected result

Issues list in any bug tracker system (publicly available), for example issues list in created GitHub repository. It's not required to push any files to repository, just create issues for empty new repository. Do not do this for current repository please.

## Requirements

1. The issue must be structured in accordance with the general recommendations for the design of QA issues. The issue must includes description as actual result, expected result, steps to reproduce, environment details, screenshot if applicable, other helpful data.
2. It is necessary to find critical bugs as well as recommendations, suggestions for enhancement of UI/UX.

## Test application

The test application is an app for finding repositories on github and saving them to favorites list. 

* Home page is the repository search page, where the user can enter a keyword and the application will search for repositories whose name or description contains that keyword. 
* The search results are presented in the form of tiles, where there are basic repository fields, a link to the repository, and a button to add the application to favorites. 
* After the search is completed, a filter is also available to the user. It's built automatically based on the search results. This filter allows user to quickly sort search results by the selected programming language.
* When adding an application to favorites, it is saved in the browser's memory (which means the list will be available even after reloading the page). 
* Favorites page contains a list of saved repositories with the ability to delete them from the list. 
* To open favorites page user is required to enter the password - 1234. Otherwise system redirects user to the Home page.

## How to launch test application

1. Install NodeJS (any latest version)
2. Download current repository, extract it and open the folder containing this file in terminal
3. Type command `npx http-server .`
   
   This will launch local server that hosts current opened folder.
4. Open browser and enter url: `http://localhost:8080` 
   
   Note: make sure you don't have any other server launched on 8080 port, otherwise pls check the link in terminal after launching http-server command and open it.
