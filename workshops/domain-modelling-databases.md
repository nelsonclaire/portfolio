# Databases - Domain Modelling using CRC Cards

Class Responsibility Collaborator cards are one approach to modelling a domain.  




### Example CRC

This is an example of using Class-Responsibility-Collaborator cards to model a domain.

#### The User Stories

```
As a customer
So I can get a bicycle
I want to withdraw a bicycle from a docking station
```

```
As a customer
So I can complete my trip
I want to dock a bicycle back at a docking station
```

```
As a customer
So I can have the best cycling experience
I want to only get working bikes from the docking station
```

```
As an administrator
So I can tell how many bikes are at each docking station
I want to get a count of the number of bikes at the docking station
```

#### Suggested CRC

```
|-----------------------------------|
|                Bike               |
|-----------------------------------|
| Responsibilities |  Collaborators |
|-----------------------------------|
| Knows if working |                |
|-----------------------------------|

|----------------------------------|
|         Docking Station          |
|----------------------------------|
| Responsibilities | Collaborators |
|----------------------------------|
| Release a bike   | Bike          |
| Dock a bike      |               |
| Count bikes      |               |
|----------------------------------|

```

#### Suggested Database Structure

```
Table: bikes
|-------------------|-----------------------|
|  id  |   working  |   docking_station_id  |
|-------------------|-----------------------|
|   1  |    true    |           1           |
|-------------------|-----------------------|

Table: docking_stations
|-----|
| id  |
|-----|
|  1  |
|-----|
```


## Learning objectives

An exercise to learn three things:

1. Explain how to use CRC cards to model a domain
2. Model a simple domain using CRC cards
3. Infer database structure from domain structure

## Instructions

Following are some user stories.

### Use CRC cards to model the domain (20 mins)

Using [CRC cards](http://agilemodeling.com/artifacts/crcModel.htm), model the domain in an Object-Oriented way.

### Create a database structure for the domain model (20 mins)

Draw out the structure of the database for the model you have built, in the following way (the example is a possible implementation of a `cohorts` table):

```
Table: cohorts

|  id  |     name     |
|---------------------|
|  1   |  "May 2016"  |
```

> You will probably need to use foreign keys and associations. There may be one or more 'join' tables involved too, in order to implement many-to-many relationships.


## User Stories

```
As a coach
So I can get to know all students
I want to see a list of students' names
```

```
As a coach
So I don't get overwhelmed with a massive list of everyone
I want to filter the list of students by cohort name
```

```
As a coach
So I can prepare for Day One and Demo Day
I want to see the start date and demo day date of a cohort
```

```
As a coach
So I can learn students' names
I want each student to give a link to the URL of a picture of them
```

```
As a coach
So I can mark certain students
I want to tag a student with many named tags (like "happy" or "ok")
```

```
As a coach
So I can see students with the same tag
I want to filter students in the list by tag name
```

```
As a student
So I can reflect on my days
I want to rate each day out of 10
```

```
As a coach
So I can get an overview of feedback
I want to see an average of the day ratings for each student
```

