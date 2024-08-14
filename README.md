# Fullstack Technical Task

Welcome to Octopus Electric Vehicles' technical task for the Fullstack Developer role. For this task you will create a small backend service that provides data to, and receives data from a front end portal.

## Background

One of our primary leasing products offers services to businesses that allows them to offer electric vehicles as an employee benefit. As part of this process lines of credit must be submitted, managed, and approved by members of our financial team.

As part of this technical task you will be implementing a backend service to manage these lines of credits and a front end application to act as an interface for internal users.

The `credit_lines.json` file provides a sample dataset with a few credit lines.

## Getting started

This project is based on Vercel's [Next.js FastAPI Starter kit](https://vercel.com/templates/next.js/nextjs-fastapi-starter), which is a hybrid Next.js + Python app that uses [Next.js](https://nextjs.org/) as the frontend and [FastAPI](https://fastapi.tiangolo.com/) as the API backend

First, install the dependencies:

```bash
yarn install
```

Then, run the development server:

```bash
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

The FastAPI server will be running on http://127.0.0.1:8000 – feel free to change the port in package.json (you'll also need to update it in next.config.js).

## Requirements

### Frontend

* Using the provided Next.js application, create a dashboard interface which:
    1. Displays all pending credit lines and allows you to click on them to see a detailed view
    2. Displays a detailed view of a credit line and provides a form to approve or deny a credit line
* The provided app uses the newer [App Router](https://nextjs.org/docs/app) but feel free to swap this out for the [Pages Router](https://nextjs.org/docs/pages) if that's what you're more familiar with
* We've purposefully not included a CSS library in this application. We suggest using a React UI library, such as [Ant Design](https://ant.design/) or similar
* Think about the structure of the app. There is no right or wrong here, we're just interested to know how you structure your application/pages/components

### Backend

* Implement a RESTful API service that provides endpoints to serve the use cases outlined in the front end requirements.
* Use a lightweight framework; we suggest [FastAPI](https://fastapi.tiangolo.com/).
* A database is not required for this task, you may either store the changes in memory or modify the provided `credit_lines.json` file on form input.
* Provide some basic tests for the key paths.

### General

* Include a README.md that explains how to setup and run the project
* Please also include in this document any improvements you would make to the application given sufficient time and any assumptions you have made.

## Submission

When you're finished, send along **one of the following** to the person that sent you the task:
* A zip of your project (complete with the `.git` folder)
* A link to a **private** repo (we will need to share which email addresses you need to add as collaborators)

## Success Criteria

* Correctness - does it meet the requirements and work as expected?
* Maintainability - is it easy for another developer to understand and expand on?
* Robustness - does it handle errors gracefully?

## Suggested Time

We appreciate your time is valuable and we suggest you don't spend more than a couple of hours on this task. Please provide notes for anything else you would have done given more time.
