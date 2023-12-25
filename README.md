<a href="https://www.postman.com/"><img src="https://assets.getpostman.com/common-share/postman-logo-horizontal-320x132.png" /></a><br />

[![Build Status](https://github.com/rafinder1/postman_labs/actions/workflows/main.yaml/badge.svg)](https://github.com/rafinder1/postman_labs/actions/workflows/main.yaml) 
 # Testing Trello REST API

This repository contains a project for testing the REST API of the [Trello website](https://www.trello.com). The project was initially created as part of a course on Udemy ([course link](https://www.udemy.com/course/postman-od-podstaw-testowanie-rest-api/)), and it has been expanded to include GitHub Actions.

## Project Description

Various functionalities on the Trello website are tested according to the documentation available [here](https://developer.atlassian.com/cloud/trello/rest/api-group-actions/#api-group-actions). The project focuses on testing operations related to creating a topic board, adding tasks to the board, modifying them, and deleting the board.

## Trello API Endpoints

The Trello API documentation is available [here](https://developer.atlassian.com/cloud/trello/rest/api-group-actions/#api-group-actions), detailing the endpoints that enable the operations tested in this project.

## Tested Functions

1. **Creating a Topic Board**
    - Using the `POST` method, a new topic board is created.

2. **Adding Tasks to the Board**
    - Using the `POST` method, tasks are added to the created board.
    - Tasks include information about the task title and its description.

3. **Modifying a Task**
    - Using the `PUT` method, a task in the board is modified.

4. **Deleting the Board**
    - Using the `DELETE` method, the previously created board is deleted.
      
5. **Retrieving Boards and Tasks**
    - Using the `GET` method, all boards and tasks are retrieved.
    - This involves fetching information about existing boards and their associated tasks.


## Environment Variables

To run the tests, it is necessary to configure environment variables that store essential information such as tokens, keys, and the base URL. The values of these variables can be found in the `trello/test_environment.json` file.

## Local Variables

The project also defines local variables storing information about the table, lists, and descriptions. These pieces of information are utilized during tests.

## Running Tests

Tests are executed using the `GET`, `POST`, `PUT`, and `DELETE` methods to call the appropriate endpoints. The tests are designed to verify the correctness of the functions defined in the project.

## GitHub Actions

The project has been extended with GitHub Actions, enabling automatic test execution after each code change. This ensures that the project is always fully functional.
