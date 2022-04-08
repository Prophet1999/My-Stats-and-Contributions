# SpringBoot Social Network Project

- Circle CI build status:
[![CircleCI](https://circleci.com/gh/Prophet1999/Social-Media-App-Backend-SpringBoot.svg?style=svg&circle-token=54d82edd98892db8d4e69740d9bee65e48242495)](https://circleci.com/gh/Prophet1999/Social-Media-App-Backend-SpringBoot)

## Introduction
This project is a continuation of the previous one. The previous project was made with pure Servlets and JSP
 technologies [details here](https://github.com/Prophet1999/Social-Network.git). I used the same
  template layout and created a new project using SpringBoot.

## Functionality
### Base
- Login / Logout
- Register
- View own profile
- View other users profiles
- Send messages
- Add and remove friends
- Accept and decline friends requests
- Update profile information
- Change password
- Search for other users
- View other users friends lists
- View last messages
- Drag and drop profile image upload
- Internationalization: English and Russian languages
- Localization

### Admin
- Make other user admin
- Block user

## Technologies used 
### Stack:
- Java 11
- Spring: SpringBoot, MVC, Data JPA, Security, DevTools, Actuator
- Maven
- H2, Mysql, ClearDb(Heroku)
- Thymeleaf
- Javascript, jQuery
- Html, CSS, Bootstrap
- Test: JUnit, Mockito

### Environment
- Heroku as CD tool
- Circle CI as CI tool
- Docker for containerization

## Application demo is available on Heroku  
Link: [https://springboot-social-network.herokuapp.com/](https://springboot-social-network.herokuapp.com/)  
Cersei is average user and Tyrion Lannister is super admin. Tyrion can't be blocked or made average admin user.

Credentials for Cersei Lannister:
 - login cersei@lannister.ru
 - password fun123  
 
Tyrion Lannister credentials:
 - login tyrion@lannister.ru
 - password fun123
 
 ## Quick start
 
 ### Required:
 - Java 11
 - Maven 
 
 ### Steps:
 1. git clone https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot.git
 2. mvn clean package -DskipTests=true
 3. cd web.social.network/target
 4. java -jar -Dspring.profiles.active=dev social-network.jar
 5. Go to http://localhost:8080

## Application profiles
- dev - profile for development, uses embedded H2 database
- qa - profile for qa testing, uses Mysql either local, or from docker container: [mysql docker container](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/master/docker/mysql%20docker%20commands.md)
- prod - profile for Heroku, uses ClearDb. ClearDb is Heroku analog of Mysql: [details](https://devcenter.heroku.com/articles/cleardb)
- docker - profile for Docker. It is created to test connection between 2 containers: mysql and social-network(spring
 boot app)
 
## Docker
This application is tested in Docker.  
I made 2 containers: mysql and social-network, and then linked them.  
Commands for images creation and containers startup may be found in the directory: [docker](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/tree/master/docker)

## Screenshots
![1](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/1.png)
![2](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/2.png)
![3](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/3.png)
![4](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/4.png)
![5](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/5.png)
![6](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/6.png)
![7](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/7.png)
![8](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/8.png)
![9](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/9.png)
![10](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/10.png)
![11](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/11.png)
![12](https://github.com/Prophet1999/Social-Media-App-Backend-SpringBoot/blob/db1e4c2e7eca1b0e15cbb3fd6f4ee0e2c37dedf0/12.png)
 
### Todo: 
- Improve test coverage. Yes, I know it is very important, but I don't have enough time.

# Social Network Jsp and Servlets Project
Maven multi-module project that simulates social network of Game of Thrones creatures.
Admin user for any profile is Tyrion Lannister as the most smart character. 

Demo may be observer on Heroku by link: [Social Network](https://dcsocial.herokuapp.com).

Tyrion Lannister credentials for login are email: tyrion@adm.ru, password: aaa123.

Heroku disables application if it is not used for a long time(more than 2 hours or more). So it may
take some time for the application initialization and start. 

## Used technologies:
* Java 8 as backend language
* Maven 3.5.4 as build tool
* Servlets 
* Jsp as template engine
* Javascript, jQuery as client-side language/library
* Java API for WebSocket(JSR 356) for notifications
* Bootstrap 3.3.7 framework for UI
* CSS for markup
* Bootstrap-notify plugin for push notifications
* JUnit for unit testing
* Mockito for servlets testing
* Jacoco for checking test coverage
* Git as version control system

## Environment
* Tomcat 8 as web-server
* H2/MySql as data bases - both supported
* Heroku as cloud and deployment tool
* Intellij Idea as IDE

## Features
* Custom / Tomcat connection pool both supported
* DAO pattern for objects access
* Auth filter for security
* Jsp tags
* Bootstrap client-side validation without library
* Drag&Drop avatar image upload without library
* Pagination without library

## Functionality
* Multi-language portal(Ru, En)
* Data initialization on start-up.
* Registration
* Login/Logout
* Administrator user with facilities to block/unblock user or make him(her) admin
* Change user settings(avatar, first name, last name, date of birth,...)
* Messages
* Push notifications about recent messages
* User search by first name and last name 
* Users pagination
* Friends requests and friendship acceptance
* Friends search
* Error page and page for a blocked user

## About the project and its purpose
This project is based on JSP and Servlets technology stack. 
The purpose of the project was to master these core java technologies for web without any framework.

### Profiles
The project has 2 profiles for build: custom and tomcat, by default custom is used.
Depending on the chosen profile the application would use custom connection pool or tomcat connection pool. 

I wanted to train my jdbc skills and write my custom connection pool. Module custom.connection is used for
this. Is is activated by default or explicitly by choosing profile "custom". If choose this profile, than all stub data
will be initialized with all game of thrones characters.

It seemed to me a good idea to have some other module for tomcat connection pool testing. 
Module tomcat.connection is used for this reason, it may be activated by choosing profile "tomcat". 
It was supposed to be a connection that should represent production connection. 
That's why this module will initialize only data base schema and admin user.

### Security
An authorization filter is used for security of the web application. It checks user's session and performs different actions
depending on the data obtained.

For disabling possibility of session hijacking and man in the middle attacks some preferences were written in the web.xml file.
A block "\<session-config\>" contains two lines "\<http-only\>" and "\<secure\>", one of them "\<secure\>" blocks local development
because it requires https connection. It is the reason why it is commented by default, but it supposed to be uncommented in
production environment. Actually, Maven may pack different web.xml file depending on profile used, but I did not want to do this.


### TODO
A lot of things should be done to make this project ready for a real production including testing.
But my aim was to prototype social network project based on Servlets and Jsp technologies. 
I made here everything I wanted to use.

And....I have no time. 

+ move project to SPA(single page application)
+ expand test coverage
+ expand validation and error messages for not only index.jsp page, but also for other pages
+ make a new module for JSON objects requesting and responding. It is a good idea to write something like a custom lib for 
information exchange in JSON format using Jackson or Gson. But it will require to change all templates. 
Additionally, all js code should be updated for parsing and sending json objects.
+ add screenshots of the project and update readme.md

# 2048 Game
(Yet another) 2048 game clone developed with Python and TKinter.

## Problem Statement
https://github.com/Prophet1999/FrontEnd-and-Dashboard-Developer/blob/14b43b6e600fd85ce3b766f6c39438e49098d345/Problem%20Statement.pdf

## Overview
About the Game
All the playing methods are the same, all you have to do is move numbers on a grid to merge them to form the number 2048; after all, you can keep on playing the game by creating larger numbers. In each move, a new number of displays (2 or 4). The player has to move the numbers using arrow keys and try to collide the same two numbers which create a new number with the total sum of the two numbers. The gameplay design is simple that the user won’t find it difficult to use and navigate.

## Requirements
* ```Python 3.5```
* ```Tkinter``` Module for Coding a user-friendly interface as introduced in class. 
 It contains many function such as create_text(), create_rectangle(), label(), button(), bind_all() that makes the user interface interactive.
 
## Design Principles
2048 is a simple mathematics puzzle game. It is a really addictive game and the main operation performed in this game is addition which makes it easy for all of us.

How to play 2048 :

1. There is a 4*4 grid which can be filled with any number. Initially two random cells are filled with 2 in it. Rest cells are empty.



2. we have to press any one of four keys to move up, down, left, or right. When we press any key, the elements of the cell move in that direction such that if any two identical numbers are contained in that particular row (in case of moving left or right) or column (in case of moving up and down) they get add up and extreme cell in that direction fill itself with that number and rest cells goes empty again.



3. After this grid compression any random empty cell gets itself filled with 2.



4. Following the above process we have to double the elements by adding up and make 2048 in any of the cell. If we are able to do that we wins.



5. But if during the game there is no empty cell left to be filled with a new 2, then the game goes over.



In above process you can see the snapshots from graphical user interface of 2048 game. But all the logic lies in the main code. So to solely understand the logic behind it we can assume the above grid to be a 4*4 matrix ( a list with four rows and four columns). You can see below the way to take input and output without GUI for the above game.

Example : 

Commands are as follows : 
'↑' : Move Up
'↓' : Move Down
'←' : Move Left
'→' : Move Right

[0, 0, 0, 0]
[0, 0, 0, 0]
[0, 0, 0, 0]
[0, 0, 2, 0]
Press the command : ←
GAME NOT OVER

[0, 0, 0, 2]
[0, 0, 0, 0]
[0, 0, 0, 0]
[2, 0, 0, 0]
Press the command : ↓
GAME NOT OVER

[0, 0, 0, 0]
[0, 0, 0, 0]
[0, 0, 2, 0]
[2, 0, 0, 2]
Press the command : →
GAME NOT OVER

[0, 0, 0, 0]
[0, 0, 0, 0]
[2, 0, 0, 2]
[0, 0, 0, 4]
Press the command : ←
GAME NOT OVER

[0, 2, 0, 0]
[0, 0, 0, 0]
[4, 0, 0, 0]
[4, 0, 0, 0]
Press the command : ↓
GAME NOT OVER

[0, 0, 0, 0]
[0, 0, 0, 0]
[0, 0, 0, 0]
[8, 2, 0, 2]
.
.
.
And the series of input output will go on till we lose or win!

Programming Approach : 

We will design each logic function such as we are performing a left swipe then we will use it for right swipe by reversing matrix and performing left swipe.
Moving up can be done by taking transpose then moving left.
Moving down can be done by taking transpose the moving right.

## Code Walkthrough
1. Board:

Variables:

Bg_color: It is a dictionary that stores background color for every cell.
Color: It is a dictionary that stores foreground color for every cell.
Window: It is the main tkinter window.
gameArea: It is a tkinter frame widget.
gridCell: It is a 4×4 integer matrix which stores the actual integer value of all the cells.
Board: It is a 4×4 grid of tkinter label widget which displays the value of the cell on tkinter window. It is also used to configure the background and foreground of the cell according to its gridCell value.
Score: It stores the current score of the player.
Rest are just flag variables.

Functions:

__init__(self): It is the constructor function. It initializes all the variables with appropriate default values like ‘0’ for gridCell, False for moved, merge and so on.
Reverse: It reverse the gridCell matrix.
Transpose: It uses zip function and takes transpose of the gridCell matrix.
CompressGrid: It moves all not empty cells to the left, so that merging can be done easily.
mergeGrid: It adds the gridCell value of two adjacent cells if they have same gridCell values.
Random_cell: It first stores all the empty cells in a list and then picks a random cell from the created list and make its gridCell value 2
Can_merge: It returns a boolean value denoting we can merge any two cells or not. We can merge two cells if and only if they hold the same gridCell value.
paintGrid: It assigns foreground and background color to each cell of the 4×4 grid corresponding to its gridCell value.

2. Game:

This class doesn’t have many variables, it only has some Boolean variables indicating game status.

Functions:

__init__(self): It is the constructor function. It initializes all the variables with appropriate default values.
start: It calls random_cell twice to assign ‘2’ to gridCell value of two random cells and then it paints the grid and after that, it calls link_keys to link up, down, left, and right keys.
Link_keys: First of all it checks if the game is already won or lost, and if it is, it executes a return statement without doing anything. Otherwise, it continues its execution.

Approach:

For left swipe, we will just compress and then merge the gridCell matrix and then if compress or merge is true (indicating the values of the matrix is affected by previous two functions), then we need to compress the grid again.
For moving up, we will take transpose then swipe left and again take transpose to return to the original order.
Moving down is same as moving up but we need to reverse the matrix.
Similarly, right is same as moving left+reverse.
After every operation, we need to check the game status, if all cells are occupied and we cannot even merge any two cells i.e. the state where no movement can change the matrix, then the game is over.

If any cell value has reached 2048, then the player is won and a message box is flashed on the screen announcing the winner.
 
 ## Screenshots

![alt text](https://github.com/Prophet1999/FrontEnd-and-Dashboard-Developer/blob/f7945f6a798eea9a458dda88195e225fb6e3a967/Screenshot%201.png)
![alt text](https://github.com/Prophet1999/FrontEnd-and-Dashboard-Developer/blob/f7945f6a798eea9a458dda88195e225fb6e3a967/Screenshot%202.png)
![alt text](https://github.com/Prophet1999/FrontEnd-and-Dashboard-Developer/blob/f7945f6a798eea9a458dda88195e225fb6e3a967/Screenshot%203.png)
![alt text](https://github.com/Prophet1999/FrontEnd-and-Dashboard-Developer/blob/f7945f6a798eea9a458dda88195e225fb6e3a967/Screenshot%204.png)

## Change from 2048 to 4096 as end number
In the original game, sometimes the new tile that pops up is a 4. Let's ignore that possibility for the sake of simplicity.

We've 16 squares in total and considering the new tile popped up at the position we chose, to make it to 4096, we need minimum these tiles:

2048, 1024, 512, 256, 128, 64, 32, 16, 8, 4, 2, 2

These can be combined from right to left to get to 4096. That's a total of 12 tiles. Since that's less than 16 (max number of tiles that can fit), 4096 is possible. Following along:

8192: 4096, 2048, 1024, ..., 4, 2, 2 Total 13
16384: 8192, 4096, 2048, ..., 4, 2, 2 Total 14
32768: 16384, 8192, 4096, ..., 4, 2, 2 Total 15
65536: 32768, 16384, 8192, 4096, ..., 4, 2, 2 Total 16
Next is 131072 which will require at least 17 tiles which can't fit on the board.

So, the largest possible tile is 65536.

EDIT: Since the game pops up some 4's at times, 131072 is still theoretically possible if the last tile that pops up is a 4 making the board look like this:

131072: 65536, 32768, 16384, 8192, 4096, 2048, 1024, 512, 256, 128, 64, 32, 16, 8, 4, 4

that's 16 tiles in total.

So now we know that 65536 is reachable in 4x4 grid so we just have to modify our result value from 2048 to 4096.
Whenever we encounter 4096 as a value on any one grid cell after each operation we just exit the program and flash "You Win".

## GitHub Repo Link
https://github.com/Prophet1999/FrontEnd-and-Dashboard-Developer

How To Run The Project?
To run this project, you must have installed Python on your PC. After downloading the project, you have to follow the steps below:

Step 1: Extract/Unzip the file if the file is zip or rar.

Step 2: Install and update all Python Modules and Libraries specially TKinter UI as it is needed for the project.

Step 3: Open latest version of Python IDEL then open "Source Code.py".

Step 4: After file is opened just run the module to see the magic happen!!!

## Scope of making this an 8x8 from 4x4
2048 is a highly popular game even though it's quite old and really simple as compared to other games today.
2048 looks very easy when you start playing it, but it gets tougher and tougher with time. 
But this is not the case with 2084 8x8. The game is really easy as you have a bigger board of 8x8 blocks to achieve the target of 2048.
It is similar to 4x4 grid except the fact that here we have to use 8x8 grid.


## Difference Between 4x4 And 8x8 Grid

The classic 2048 game has a 4x4 board. And the user has to make a single tile display 2048 as the final number in order to win the game. 4x4 tiles make the game very hard and you have to think twice before taking the next step. But this is not the case with 2048 8x8. 2048 tile can easily be obtained even if you randomly move the tiles. The reason being, the tiles are four times as compared to what we get in 2048.

## Thoughts  Probable solutions and Problems faced while designing the solution
Thoughts / Probable solutions / Problems faced while designing the solution

1. The Matrix manipulation and handling was tricky and difficult.
2. There is no way to optimize the operations on the matrix.
3. Lots of research needed for the algorithm.
4. Minimum Understanding while playing the game.
5. Adding the scores and leaderboards was a time taking process.

Sentiment Analysis Using Neural Networks
In PYTHON (April–May 2021)

It is an attempt to monitor and rate 
the views , reviews and opinions of a 
particular product or service based on 
the language , phrases and tone used 
to judge and recommend it for other 
customers. 

Azure QuickStarts Projects
==========================

A collection of quickstart projects demonstrating core Microsoft Azure services and their APIs.

[Download from Visual Studio Extension Gallery](http://visualstudiogallery.msdn.microsoft.com/f56f321d-e2a7-4ee1-864e-5752617dbf1d)

# Development Environment

In order to contribute to the Azure QuickStarts you will need the following tools install on your machine.

+ [Visual Studio 2013](http://go.microsoft.com/?linkid=9832446&clcid=0x409)
+ [Visual Studio 2013 SDK](http://go.microsoft.com/?linkid=9832352)
+ [Azure SDK & Tools](http://go.microsoft.com/fwlink/p/?linkid=323510&clcid=0x409)
+ [SideWaffle Template Pack](http://visualstudiogallery.msdn.microsoft.com/a16c2d07-b2e1-4a25-87d9-194f04e7a698)
+ [NuGet](http://visualstudiogallery.msdn.microsoft.com/4ec1526c-4a8c-4a84-b702-b21a8f5293ca)
+ [Microsoft Azure Management Libraries](http://www.nuget.org/packages/Microsoft.WindowsAzure.Management.Libraries) <small>(MAML)</small>

# Getting Started

I'm glad that you're interested in providing a sample for the Azure QuickStarts, here are some quick notes to help you along your way.

<a name="what-is-a-sample"></a>
## What is a Sample?

A sample is meant to be the simplest possible example of the use of a service. Essentially the point is to exercise the API/SDK for a particular Service or if needed provide a link to a more advanced sample.

> **Example**
> 
> *Blob Storage Sample*
>
> + Create Storage Account
> + Create Container
> + Create Blob
> + Modify Blob Properties/Metadata
> + Read Blob 
> + Delete Blob
> + Delete Container
> + Delete Storage Account

## Where do I put things? <small>(aka Directory Structure)</small>

This provides a general reference as to where a sample should be placed. If in doubt see the [Documentation](http://azure.microsoft.com/en-us/documentation/) under Documentation by Service section.

### App Services
+ Samples for services which provide support an application accomplish a given task.

### Compute
+ Samples for services which provide an endpoint for an application.

### Data Services
+ Samples for services which provide storage for an application.

### Deployment and Management
+ Samples for Automating the creation and management of services using an API/SDK.
	
### Network Services
+ Samples for services which connect Compute Services using Network or DNS.

## How do I build a sample?

### App Services
+ Console Application which shows service functionality
+ Reference Online Documentation

### Compute
+ Reference Online Documentation

### Data Services
+ Console Application which shows service functionality
+ Reference Online Documentation

### Deployment and Management
+ Console Application which uses:
	+ [MAML](http://www.nuget.org/packages/Microsoft.WindowsAzure.Management.Libraries)
	+ [Azure Resource Management API](http://msdn.microsoft.com/en-us/library/azure/dn790568.aspx) (only if not defined in previous)
	+ [Service Management API](http://msdn.microsoft.com/en-us/library/azure/ee460799.aspx) (only if not defined in previous)

### Network Services
+ Reference Online Documentation

## How to prepare my sample for inclusion

### I can write a simple sample

1. Right click on the sample project, select **`Add > New Item > SideWaffle Project Template Files`**
1. Provide the **`_Definitions/_project.vstemplate.xml`** file with an appropriate Name and Description for the project template
	+ Be sure to include the `<WizardExtension>` xml snippet (below) as a child of the `<VSTemplate>` element.
		<pre>
		&lt;WizardExtension&gt;
	      &lt;Assembly&gt;ProjectWizard, Version=1.0.0.0, Culture=Neutral, PublicKeyToken=f30ae472f039a534&lt;/Assembly&gt;
	      &lt;FullClassName&gt;ProjectWizard.Wizard&lt;/FullClassName&gt;
	  	&lt;/WizardExtension&gt;
		</pre>
1. Update `_Preprocess.xml` as needed (generally not)
	+ Ensure the attribute `Path` in the `TemplateInfo` element describes where the Project Template should show in the **`File > New Project`** dialog
	+ Add a key value pair (replacement token) to the `Replacements` element if the project contains code. 
		+ Key value pairs can be removed from the `Replacements` element if it provides a link to some documentation.
1. Update sw-file-icon.png with the appropriate azure service logo which will be used for the template.

> **I need to create a Multi-Project Template!**
>
> See  [How to create a multi-project temlate](https://github.com/ligershark/side-waffle/wiki/How-to-create-a-multi-project-template). If you get stuck you can contact [Sayed Ibrahim Hashimi](https://twitter.com/sayedihashimi).

### I can't prepare a simple sample

If there isn't a public API surface which is [easy to explore via a QuickStart](#what-is-a-sample), it's still valuable to add a template which provides a redirect to an online sample (maybe from azure.microsoft.com).

This is valuable because the service will still be discover-able by Developers from within Visual Studio.

Follow the steps from above with these additional steps:

1. Add a `WizardData` element as a child of the `<VSTemplate>`	element.

	<pre>
	&lt;WizardData&gt;
	  &lt;navigation&gt;
	    &lt;navigate path="[path-to-tutorial]" generateProject="false" /&gt;
	  &lt;/navigation&gt;
	&lt;/WizardData&gt;
	</pre>

2. Delete the `AssemblyInfo.cs` file from the `Properties` folder.
3. Delete the `Program.cs` file from the project.
4. Delete the `app.config` file from the project.

# Stock Market Analysis and Prediction

## Introduction
Stock Market Analysis and Prediction is the project on technical analysis, visualization, and prediction using data provided by Google Finance. By looking at data from the stock market, particularly some giant technology stocks and others. Used pandas to get stock information, visualized different aspects of it, and finally looked at a few ways of analyzing the risk of a stock, based on its previous performance history. Predicted future stock prices through a Monte Carlo method!

## Purpose
The purpose of this project is to comparatively analyze the effectiveness of prediction algorithms on stock market data and get general insight on this data through visualization to predict future stock behavior and value at risk for each stock. The project encompasses the concept of Data Mining and Statistics. This project makes heavy use of NumPy, Pandas, and Data Visualization Libraries.

<a href="https://www.scaler.com/event/hackx/">
  <p align="center">
    <img src="https://i.imgur.com/QbwPFZM.jpg" />
  </p>
</a>


## How to submit:
- Upload your code somewhere on the internet. This can be to a GitHub repository ( preferred ), a zip file on cloud storage, anywhere: as long as it is accessible by the judges. You will provide a link to this in the next steps.
- Login to your GitHub account. 
- Make sure that the following are taken into consideration before submitting ( failure to do so will result in disqualification ) : 
  1. Make sure you have your code link ready 
  2. You should be ready with your PPT/Document of your project.
       -  [Sample PPT](https://docs.google.com/presentation/d/1tzXTgzFN6dMM5pMjtniSwiO-Q_4PR_nPmLOOn9S8YdI/edit?usp=sharing)
  4. Demo Video for the project - 
       - Tell us about your project
       - Demo of your project
       - Video must be in English
       - File name should be TeamName_HackX
  5. Demo Link ( if applicable ) - Hosted / Live link of the prototype
- Start a [new submisison issue](https://github.com/scaleracademy/hackx-submissions/issues/new/choose).
- Complete the template. 
- Submit the issue (one per team). 
- Success 🎉

## Problem Statements & Submission Guidelines 
- [Problem Statements](https://scalerdiscord.notion.site/HackX-by-Scaler-Submissions-1d5d77a36e4e48888f60ecd449c7b86a)
- [Walkthrough Video](https://bit.ly/hackxsubmissions)


## Rules
Kindly go through the [Rules](https://github.com/scaleracademy/hackx-submissions/blob/main/rules.md).

## Code of Conduct
Kindly go through the [Code of Conduct](https://github.com/scaleracademy/hackx-submissions/blob/main/coc.md).

## Submissions
All the Project Submissions have to done by making an issue in this repository. The guidelines to followed for the same have been mentioned below:
1. The **Team Leader** has to open up an Issue for project submission using their GitHub Account [here](https://github.com/scaleracademy/hackx-submissions/issues/new/choose)
2. The **Issue Template** should be strictly followed. A submission not following the same would be termed as an INVALID SUBMISSION.
3. Specify appropriate project field from the checklist, please delete anything that does not matter to you.
4. Only a **single issue** has to be made for each individual project, Multiple submissions will be termed as INVALID SUBMISSION.

## Project Theams:
Choose from the below themes
<p align="center">
  <img src="https://i.imgur.com/4FDB4od.jpg" />
</p>


## FAQs
You can also refer to the [FAQs](https://scalerdiscord.notion.site/scalerdiscord/Frequently-Asked-Questions-ca204bb1489140dfabe9218536aa8923).

## Contact Us
For all communications and queries, you can join our [Discord Server](https://discord.gg/4pR79vEKUE).

# SpringBoot Social Network Project

- Circle CI build status:
[![CircleCI](https://circleci.com/gh/dmcheremisin/SpringBootSocialNetwork.svg?style=svg&circle-token=54d82edd98892db8d4e69740d9bee65e48242495)](https://circleci.com/gh/dmcheremisin/SpringBootSocialNetwork)

## Introduction
This project is a continuation of the previous one. The previous project was made with pure Servlets and JSP
 technologies [details here](https://github.com/dmcheremisin/SocialNetwork). I used the same
  template layout and created a new project using SpringBoot.

## Functionality
### Base
- Login / Logout
- Register
- View own profile
- View other users profiles
- Send messages
- Add and remove friends
- Accept and decline friends requests
- Update profile information
- Change password
- Search for other users
- View other users friends lists
- View last messages
- Drag and drop profile image upload
- Internationalization: English and Russian languages
- Localization

### Admin
- Make other user admin
- Block user

## Technologies used 
### Stack:
- Java 11
- Spring: SpringBoot, MVC, Data JPA, Security, DevTools, Actuator
- Maven
- H2, Mysql, ClearDb(Heroku)
- Thymeleaf
- Javascript, jQuery
- Html, CSS, Bootstrap
- Test: JUnit, Mockito

### Environment
- Heroku as CD tool
- Circle CI as CI tool
- Docker for containerization

## Application demo is available on Heroku  
Link: [https://springboot-social-network.herokuapp.com/](https://springboot-social-network.herokuapp.com/)  
Cersei is average user and Tyrion Lannister is super admin. Tyrion can't be blocked or made average admin user.

Credentials for Cersei Lannister:
 - login cersei@lannister.ru
 - password fun123  
 
Tyrion Lannister credentials:
 - login tyrion@lannister.ru
 - password fun123
 
 ## Quick start
 
 ### Required:
 - Java 11
 - Maven 
 
 ### Steps:
 1. git clone https://github.com/dmcheremisin/SpringBootSocialNetwork.git
 2. mvn clean package -DskipTests=true
 3. cd web.social.network/target
 4. java -jar -Dspring.profiles.active=dev social-network.jar
 5. Go to http://localhost:8080

## Application profiles
- dev - profile for development, uses embedded H2 database
- qa - profile for qa testing, uses Mysql either local, or from docker container: [mysql docker container](https://github.com/dmcheremisin/SpringBootSocialNetwork/blob/master/docker/mysql%20docker%20commands.md)
- prod - profile for Heroku, uses ClearDb. ClearDb is Heroku analog of Mysql: [details](https://devcenter.heroku.com/articles/cleardb)
- docker - profile for Docker. It is created to test connection between 2 containers: mysql and social-network(spring
 boot app)
 
## Docker
This application is tested in Docker.  
I made 2 containers: mysql and social-network, and then linked them.  
Commands for images creation and containers startup may be found in the directory: [docker](https://github.com/dmcheremisin/SpringBootSocialNetwork/tree/master/docker)

## Screenshots
![1](https://raw.githubusercontent.com/dmcheremisin/SpringBootSocialNetwork/master/screenshots/1.png)
![2](https://raw.githubusercontent.com/dmcheremisin/SpringBootSocialNetwork/master/screenshots/2.png)
![3](https://raw.githubusercontent.com/dmcheremisin/SpringBootSocialNetwork/master/screenshots/3.png)
![4](https://raw.githubusercontent.com/dmcheremisin/SpringBootSocialNetwork/master/screenshots/4.png)
![5](https://raw.githubusercontent.com/dmcheremisin/SpringBootSocialNetwork/master/screenshots/5.png)
![6](https://raw.githubusercontent.com/dmcheremisin/SpringBootSocialNetwork/master/screenshots/6.png)
![7](https://raw.githubusercontent.com/dmcheremisin/SpringBootSocialNetwork/master/screenshots/7.png)
![8](https://raw.githubusercontent.com/dmcheremisin/SpringBootSocialNetwork/master/screenshots/8.png)
![9](https://raw.githubusercontent.com/dmcheremisin/SpringBootSocialNetwork/master/screenshots/9.png)
![10](https://raw.githubusercontent.com/dmcheremisin/SpringBootSocialNetwork/master/screenshots/10.png)
![11](https://raw.githubusercontent.com/dmcheremisin/SpringBootSocialNetwork/master/screenshots/11.png)
![12](https://raw.githubusercontent.com/dmcheremisin/SpringBootSocialNetwork/master/screenshots/12.png)
 
### Todo: 
- Improve test coverage. Yes, I know it is very important, but I don't have enough time.
