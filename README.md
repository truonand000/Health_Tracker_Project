# Health Buddies
By Andrew Truong, Nancy Tran, and Sean Hellman

## Purpose
Our project is a groupware application that aims to encourage people to collaborate with one another to achieve a healthier lifestyle. We plan to achieve this by creating a space where simple actions such as meal planning, exercise, and personal health-related goals/achievements can be tracked and shared with friends/family. 

## Features
### Meal and Fitness Tracking
Connect to nutrition API to provide information about meals that users can search up, save, and track daily.
User also can input their exercise and the duration of their exercise. 
### Communication Channel: Messenger
Users have the ability to start a chat room with other existing users, so that they can chat about their improvements and potentially schedule health related events (such as checking out a new healthy restuarant, exercising together, etc.)
### Metrics/Goal profile
Users have a set profile indicating their goal and several metrics such as their exercise streak.

## Limitations
We decided to center this app around mobile use only. Due to time constraint, we weren't able to implement a number of features we had in mind. These features include:
- an event scheduler
- ability to share profiles with other users
- calorie accumulator per day
- ability to scroll to previously logged days
- data visualization of food and exercise logging
- ability to customize your goals
- creating an account and account authentication
- feedback to users in chatroom (ex. read reciept, other user currently chatting)
- our implementation only supports single person direct messaging, it would be ideal to eventually allow group messaging
- also, our log out is a little bit buggy

## Technology
This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app). We used Firebase to manage our data, redux for state management, https://developer.edamam.com/food-database-api-docs as our nutrition API, and socket.io as our server-client framework. 

We successfully deploy our application on Heroku, which can be found here: [link to app](https://healthyman.herokuapp.com/). It does, however, have a few bugs that have yet to be worked out. There were several attempts to fix these bugs (which are related to chat and profile), but our server would not run on Heroku after these changes so we decided to deploy an older version that did work.

## Groupware Principles
- Mostly asynchronous service, but has some synchronous features such as messaging.
- Mostly remote service.
- Communication is supported through chat application.

## How we split up our work
- Sean implemented the ability to input meals/fitness, data fetching from the nutrition api, and saving users' input in firebase.
- Andrew implemented the user profile, the backend of setting up individual chat rooms using a server and clients, and saving new messages in firebase.
- Nancy implemented the navigation bar, onboarding, and the UI and some backend in the chatroom/messaging.

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

## Available accounts
Currently there are 4 possible accounts you can log in as. For expert users testing we recommend logging in as:
- username: sean password: sean
- username: nancy password: nancy
- username: andrew password: andrew<br>
For novice user testing, log in as:
- username: newuser password: newuser
