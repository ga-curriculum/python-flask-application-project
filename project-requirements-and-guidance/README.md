<h1>
  <span class="headline">Python Flask Application Project</span>
  <span class="subhead">Project Requirements and Guidance</span>
</h1>

## Overview

**Objective**:

Create a basic Flask application that reads data from either a `.csv` file or an external API and displays it to the user through read-only routes. This project will help you improve your Flask skills, learn to handle external data in Python, and explore serving dynamic content via APIs or HTML templates.

**Scope and Complexity**:

This Flask project focuses on reading and displaying data and is designed to take approximately 15 hours to complete.

You'll develop a Flask application that presents data from a `.csv` file or an external API using read-only routes. You can add complexity to your application by performing interesting data operations or integrating external data through API calls.

**_You will work individually on this project_**.

> ❗️ As a reminder, General Assembly has a zero-plagiarism policy. **_Your project's code must be substantially yours_**. Do not copy code from similar projects or other sources. However, using code from the internet to accomplish generic tasks is okay - for example, a line of code that replaces a character at a specific position in a string.

A printable version of the project requirements can be found [here](./assets/project-requirements.pdf).

## Technical requirements

### Minimum requirements

> ✅ Any items marked incomplete in this section will result in the project receiving a failing grade.

Your Application must have the following functionality:

1. **Data Handling:**

   - The application reads and parses a `.csv` file correctly or successfully fetches and processes data from an external API.

2. **Data Presentation:**

   - The application presents data through routes that are accessible and user-friendly, whether viewed in a browser or via Postman.
   - No errors are present when accessing API endpoints or web pages.

3. **No Write Operations:**

   - The application does not include any routes that allow for creating, editing, or deleting data.

4. **Route Documentation:**

   - The README file includes a table documenting all available routes. The table lists the route path, HTTP method, description, and any parameters required.

   **Example Table for README**:

   | **Route**      | **HTTP Method** | **Description**                         | **Parameters**   |
   | -------------- | --------------- | --------------------------------------- | ---------------- |
   | `/data`        | GET             | Returns all data from the CSV or API.   | None             |
   | `/data/<id>`   | GET             | Returns a specific item by ID.          | `id` (integer)   |
   | `/data/search` | GET             | Searches data based on query parameters | `query` (string) |

## Detailed Technical Requirements

Your application should:

1. **Read Data from a CSV File or an external API**:

   - **Option 1**: Load data from a `.csv` file. The data can be of any kind—be creative! For example, you might use a dataset related to books, movies, or any other topic of interest.
   - **Option 2**: Pull data from an external API. Choose an API that provides data relevant to your application idea.
   - **Option 3**: Do both. If you chose the CSV option for your primary data source, you can optionally include an API call within your Flask routes to fetch additional external data and present it alongside the CSV data.

2. **Use Read-Only Routes**:

   - Implement routes that allow users to view the data from the CSV file or API.
   - The routes should be strictly read-only—no data creation, editing, or deletion should be allowed.

3. **Present Data to the User**:

   - Choose how you want to present the data:
     - **Option 1**: Build a back-end only API that sends back JSON data. The data should be viewable directly in a browser or through tools like Postman.
     - **Option 2**: Use Jinja templates to populate HTML pages with the data. This option allows you to create more formatted and user-friendly web pages.

## Code convention and UI/UX requirements

> ✅ More than one item marked incomplete in this section will result in the project receiving a failing grade.

- The code must be well-organized and modular, with functions handling specific tasks.
- The code should follow Python best practices and be well-documented with comments where necessary.
- Error messages should be clear and informative, guiding users to correct their input.

## README requirements

> ✅ More than two items marked incomplete in this section will result in the project receiving a failing grade.

- The app's name.
- A brief description of your app and its functionality.
- A table documenting _all available routes_. The table lists the _route path_, _HTTP method_, _description_, and any _parameters required_.
- A _Getting started_ section. This section should include instructions on how to interact with your app.
- A _Technologies used_ section. This section should list the principal technologies used by your application, for example, Python and any major frameworks or libraries.
- If necessary, an _Attributions_ section. This section should include links to any external resources (such as libraries or assets) you used to develop your application that require attribution. You can exclude this section if it does not apply to your application.

## Evaluation

Your instructional team will evaluate your project after the project's due date. Your instructors will use the above guidelines to determine whether or not your project meets all of the minimum requirements.

If there is a specific section of code that you would like an instructor to provide additional feedback on, please ask!

## Guidance

### Getting started

Here are some quick tips to get your project started:

- Discuss your app idea with an instructor to get feedback before you dive too deep into planning.
- **_Keep it simple._** Minimum Viable Product (MVP) functionality that works well is better than extra functionality added to an app with bugs
- Prioritize and implement functionality step-by-step, one at a time. Develop features in a way that allows you to test as you go - try your best to follow the flow of data through your app.
- Regularly review the project requirements to ensure you're on track to pass the project. A printable version of the project requirements can be found [here](./assets/project-requirements.pdf).
- Add comments to your code where it makes sense to do so. Most code is self-documenting, and you shouldn't add comments explaining the obvious. Ideally, comments should explain the **_why_** of code where it's necessary.

### Project assistance

Your instructor team will provide guidelines for reaching out for help during the project.

## Project inspiration

Need some ideas to get started?

_Here are some ways you can incorporate CSV data with an external data API:_

<br>

#### **Currency Conversion Tracker**

Create a Flask app that reads transaction data from a `.csv` file and converts the amounts to a single currency using real-time exchange rates from an API.

**Description**:  
Upload a `.csv` with transactions in various currencies, convert them to a preferred currency using an API, and display the results with both original and converted amounts.

---

#### **Travel Cost Analyzer**

Develop a Flask app that reads a `.csv` file of destinations and activities to calculate the total budget needed for a trip using real-time travel costs from APIs.

**Description**:  
Upload a `.csv` with trip details, fetch travel costs using APIs, and calculate the total trip budget, providing a detailed breakdown of expenses.

---

#### **Real Estate Investment Calculator**

Build a Flask app that reads property details from a `.csv` file and calculates potential investment returns using current market data from an external API.

**Description**:  
Upload a `.csv` with property information, fetch market data from an API, and calculate key investment metrics like ROI, presenting the results clearly.

---

#### **Weather Data Logger**

Create a Flask app that reads a `.csv` file containing dates and locations, then retrieves historical or current weather data for those locations using a weather API.

**Description**:  
Upload a `.csv` with dates and locations, fetch weather data from an API, and display the weather conditions for each date and location in a user-friendly format.

---

#### **Movie Recommendation App**

Build a Flask app that reads a `.csv` file containing user movie ratings and uses an external API to recommend similar movies.

**Description**:  
Upload a `.csv` with movie ratings, fetch recommendations from a movie database API (like TMDb or OMDb), and display a list of recommended movies based on user preferences.

---

#### **Book Price Tracker**

Develop a Flask app that reads a `.csv` file of book titles and checks their prices across multiple online stores using an API.

**Description**:  
Upload a `.csv` with book titles, fetch current prices from online stores using an API, and display a comparison of prices for each book to help users find the best deals.
