# Jog Logger


## Project Description 

Users will create an account to track and store their running exercises. After going on a run, users may enter in the date, distance (in miles), total time, and calories burned on their run. The home page will consist of all runs stored in chronological order and will display the distance and average mile speed for each run. The top section shows the user their avergage mile time and their fastest mile time. EXTRA: At the end of every month, the top will display the user's total calories burned and miles ran for the month.

## Visual

https://xd.adobe.com/view/12f54b28-3956-4d8e-8a20-6ec7453fbc7f-47a6/
(Add new adobe file here)


## Schema

``` 
const Entry = new Schema(
  {
    distance: { type: String, required: true },
    duration: { type: String, required: true },
    calories: { type: String, required: true }
  },
  { timestamps: true }
)
const User = new Schema(
  {
    name: { type: String, required: true },
    email: { type: String, required: true },
    password_digest: { type: String, required: true }
  },
  { timestamps: true }
)
```

## Component Diagram

[Component Hierarchy](https://whimsical.com/jog-logger-app-QzwYytCNAvUEgYsBwa6uBJ)

## MVP

- Authentication
- Home page which displays all run entries and an add button
- Form for new run entry
- Average mile time for all miles for that user dislayed at the top of home
- Displays calories burned in the last 30 days
- Server Back-end stores all entries and users
- Front-end deployed to netlify/surge

## Post MVP

- Landing screen when opening the app that fades into the login or home page if they are logged in already
