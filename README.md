# Campus Maps

Interactive Maps for Colleges and Universities all around the world.

## Problem

Colleges and Universities tend to be located on huge plots of land where the buildings are inaccessible by vehicles. Usually people have to walk to buildings through a series of sidewalks that are usually poorly labeled. In addition students are given a brief overview where everything is located using either overly detailed, or simplistec.   campus maps. Thousands of students, and faculty members every semester walk into school completely lost and unaware of how to get around campus.

We believe that this can be resolved with an interactive map that can give students directions to their classes or any of the facilities on the campus. 

## Other Obeservations

One thing we noted when discussing the application was that there are other use cases for an interactive map application. 

### Class Specific Updates

Often students will get an email from one of their professors to tell them that the class has been relocated to a different building or classroom. Usually the students don't know until they get to the classroom where they find a paper note sending them to another building. Imagine if you were on crutches and you have to walk from one side of the campus to another because you weren't informed. 

### Alerts For Faculty

Imagine if the professors of certain classes can send an alert that all the other faculty could see. 

- A ⚠️ symbol can represent a safety issue in the classroom. 
- A 🖥 symbol can represent an issue with the computers in the classroom.
- A ❄️ symbol can be something related to the air termperature or comfort.
- A 📩 symbol can be an alert for students to read, like class canceled.

### Directions

We intend to use service workers in this application so that students / faculty could use it in areas with poor data connections. With this we can rely on the application to give us offline directions from one class to the other. I imagine we could have it calculate the shortest route as well. 

## The Application

At the moment we intend to build the application using:

- React
- React Native for Mobile
- Express
- MongoDB
- Handlebars (server side rendering)
- Mocha / Chai or Jest
- Service Workers
- Google Maps API
- Docker
- CICD
- Travis CI

### Wireframes

#### Homepage
![Homepage](https://cdn.appstorm.net/windows.appstorm.net/files/2012/07/Balsamiq-Mockups-Bahoo-Maps.png)

### Running the Application

1. Clone the app ```git clone https://github.com/AppLyfe/campusMaps.git```
2. Go into the cloned directory ```cd campusMaps```
3. Install a crap load of node modules in the main _server_ directory with ```yarn``` command.
4. Go into the client folder and install those dependencies as well. ```cd client``` yes the React Folder is called _client_.
5. Go back to the main directory and lets run some scripts.


#### Start

```yarn start``` or ```npm run start```
Runs node server file located in ./bin/www **Running on Port 5000**

#### Server

```yarn server``` or ```npm run server```
Runs a nodemon server that monitor's any changes to the express server, and re-starts the server on save. **Running on Port 5000**

#### Dev

```yarn dev``` or ```npm run dev```
Runs a nodemon server that monitor's any changes to the express server, and it runs the React server / client concurently. 

Express server **Running on Port 5000**
React server **Running on Port 3000**

#### Other Scripts

Maybe we should set up other scripts in the main package.json like build, and the rest of the react scripts. ....Later

## To Do: 

Tasks and tickets will be hosted on the GitHub Projects board.

### Commiting Code

1. First things first make your code / repo is up to date ``` git pull```
2. Before you start working create a branch with the name of the ticket you are working on. For instance, if you are working on a ticket called _googleAPI_ you should make a branch named that way ```git checkout -b googleAPI``` (checkout lets you use that branch and -b lets you create it at the same time)
3. If you cloned the project correctly the origin should be our github repo, you could always check with ```git remote -v``` to see where you are going to be pushing to, and if your remote is set to the right repo. It should look something like this:

    ```origin	https://github.com/AppLyfe/campusMaps.git (fetch)```

    ``` origin	https://github.com/AppLyfe/campusMaps.git (push)```

4. Then you could add your files ```git add .```
5. Commit ```git commit -m "This is what I did for this API```
6. Push ```git push origin googleAPI``` _origin_ is where are you pushing to... and _googleAPI_ is the branch you are pushing to.
7. Then finally you will see your code online on github and you will have to do a Pull Request against the branch that you want to send your code to. If we are doing continous development it is going to be the _development_ folder. If we aren't or if what you are pushing is going straight to _master_ then you do the PR against master. You shouldn't be able to push to master but you should be able to push to a seperate branch. ToDO: ---SCREENSHOTS---
8. We are probably going to delete the branch after it gets merged so that you don't use a stale branch. The next thing you work on should go on to a new branch.
9. There will be times when your branch goes stale, because the repo online has changes you don't have. Lets say somebody finished the css and you want to have it in your branch. To do that we will have to rebase, and that is a pain in the ass. 

### Updating Stale Branch
TODO: ---WRITE THIS---

