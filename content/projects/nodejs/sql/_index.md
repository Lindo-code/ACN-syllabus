---
_db_id: 282
content_type: project
flavours:
- javascript
learning_outcomes:
- web_dev_database_connection
- web_dev_database_queries
- wed_dev_enviromental_variables
- web_dev_docker_configuration
- web_dev_database_management_system
- web_dev_indepth_tdd
prerequisites:
  hard:
  - sql/shop-project
  - topics/node-and-sql/
  - projects/nodejs/file-io
  - topics/unit-testing-mocks-and-spies
  - topics/clean-code/sql
  soft: []
ready: true
story_points: 5
submission_type: repo
tags:
- node
- sql
title: Node & SQL assignment
---

You are required to create a backend service that will help capture basic information about prospective students who come to inquire here at Umuzi.

## database setup

1. Set up a Postgresql database on your computer. Please use Docker to do this. You can find more information here: {{< contentlink path="docker/intro-to-docker" >}}.
2. Create a table inside the database and name it Visitors.
3. The table must contain the following fields :

- id: This should be automatically generated by SQL
- visitor name
- visitor's age
- date of visit
- time of visit
- the name of the person who assisted the visitor
- comments

## Helloworld

Before you dive into anything too intense, let's make sure that you can get node to connect to your database. Can you get this Node script to run:

{{< code_snippet "helloworld.js" >}}

## Functionality

Create a single index script with the following functions:

- `addNewVisitor`. This should save the Visitor into the database
- list all visitors. This should return an array of all the visitor names and ids
- delete a visitor
- update a visitor
- view one visitor: given a visitor's id, return all information about that visitor
- delete all visitors
- view last visitor: return the last visitor's id in the database

## NOTE

You will be expected to properly test your code. You can use whatever testing framework you want. If you use something that isn't taught at Umuzi please justify your choice (if you found something cool we might incorporate it into the syllabus)

## Resources

- https://www.guru99.com/introduction-to-database-sql.html
- https://www.w3schools.com/sql/sql_intro.asp

## Instructions for reviewers

- Connection strings should never be exposed. Ensure that the `.dotenv` module has been utilized.
- The `.dotenv` file should not be present in the repo and should be specifically excluded through the use of `.gitignore.`
- Ensure that Docker and docker-compose have been used. The `docker-compose.yml` file should be at the root of the project.
- Ensure that the proper data type is returned for each function.
- If used in the project, Ensure that `Pool.connect || Client.connect` and `Pool.end || Client.end` is used correctly. There is generally no need for opening and closing your connection inside every function.
- Ensure the use of `return`, not `console.log`.
- When it comes to testing for this project, have a look at {{< contentlink path="topics/unit-testing-mocks-and-spies" >}} , and make sure that mocks and spies are utilized properly.
- did the learner follow all the clean coding practices described in {{< contentlink path="topics/clean-code/sql" >}}