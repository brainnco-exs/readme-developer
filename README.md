# Exercise for Developers

## Introduction

This is our programming exercise. Our goal is to evaluate your programming skills level and then make an interview with better information about you. After you open a pull request to the `master` branch in your private repository, we will:

1. Do your code review
2. Share our evaluation based on the list below
3. Invite you to an interview

## What we will evaluate

We want to evaluate your ability to deliver clean code with sufficient documentation for other developers to understand what you did and actively contribute to the project.

1. `README.md` is well written, with the instructions needed to run the application, etc.
2. The code is well written, clean and cohesive.
3. Implementation of the solution is working as expected.
4. There are well written automated tests (i.e., the unit and integration tests cover the expected behavior).
5. There is linter/static code analysis.

For **back-end exercises**, we will also evaluate important aspects for this area.

6. RESTful API design is implemented, correctly using the `HTTP` verbs and the proper `Status Code`.
7. An API documentation is available by an expressive and maintainable format, for its clients, e.g., Postman.

For **front-end exercises**, we will also evaluate important aspects for this area.

6. There is good usage of Javascript, HTML5 and CSS3.
7. The screens were implemented exactly as it is in the wireframes provided, e.g., the position of the elements on the screen.

### Programming language

You may choose the programming language of your preference.

### How to share your code with us

We want you to experience how we work on a daily basis. That's why we ask you to use a standard gitflow as follows below.

1. Create a `README.md` file describing how to configure your project, containing the commands that must be executed to run the software and the tests.
2. Open a new pull request to the `master` branch of the private repository that we have invited you to contribute.
3. If you have made use of any Linter (esling, rubycop, creed, etc.), send the file together with the project.

## Exercise

### Introduction

GitHub is a social network of programmers that has an interesting functionality that allows you to ["star" other users repositories](https://help.github.com/en/articles/saving-repositories-with-stars). The users activate that just by pressing a button. But it has some limitations when we consider GitHub heavy users.


### Use case

You are an active GitHub user, who is always looking for new projects and enjoying those who are interesting. You would like to be able to add a label or tag to a repository so that it can be found later. For example, you've found a repository called `react` and you would like to add ` javascript` and `frontend` tags to it. Because GitHub does not have this functionality, you want to build a simple system that can help with this task.

### Global requirements

- Retrieve starred repositories of a user's GitHub profile.
- Manage retrieved repositories tags (i.e., add, edit, delete).
- Filter repositories by tags.
- Suggestion of tags for repositories.

### User stories

**Story 1: Obtain starred repositories**

```
As a GitHub user
I want to provide my username
So that I can see all repositories that I've starred
```

Requirements

- You should get starred repositories using the GitHub Public API.
- The information that must be retrieved is: repository ID, repository name, description, HTTP URL, and language.

**Story 2: Add tags to repositories**

```
As a GitHub user
I want to be able to add tags to repositories that I've starred
So that I can easily find them later by tags
```

Requirements

- A repository can not have duplicated tags.

**Story 3: Search repositories by tags**

```
As a GitHub user
I want to be able to search by a specific tag
So that I can see my starred repositories that I've added this tag
```

Requirements

- The search field should work for queries with strings in half (e.g., by typing "doc", the "docker" and "ex_doc" repositories must be returned).

## Instructions

In order to implement the user stories listed above, please, **choose one of the following instructions: back-end, or front-end**. If you want to make both, we will consider this an extra point and effort, but it is *not* mandatory.

### Option 1: Back-end instructions

- Your REST API must be implemented using JSON.
- Each action must have its specific route respecting the convention of `http verb` and `status code`.
- Repositories and their tags must be persisted at a local database.
- Using Docker to configure the environment is recommended, but not mandatory.

### Option 2: Front-end instructions

- The user interfaces (UI) must follow the design provided below:
1. [Home](wireframes/01.png)
2. [Loading](wireframes/02.png)
3. [Repositories list](wireframes/03.png)
4. [Manage tags](wireframes/04.png)
5. [Filter by tags](wireframes/05.png)
- Repositories and their tags must be persisted in the user's local storage.
