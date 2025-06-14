# Wanderlust - Rental Platform (Phase One)

Wanderlust is a full-stack rental platform inspired by Airbnb, where users can explore, list, and manage property rentals. This README covers the completion of **Phase One**, which includes setting up the backend structure, building RESTful routes, integrating client-side validation, and adding error handling with a fully styled interface.

## Phase One Overview

The first phase of development is divided into three key parts:

### Part 1: Core Backend Setup & CRUD Functionality

* Basic Project Setup

  * Initialized project with Express, Mongoose, and EJS.
  * Configured method-override and necessary middleware.

* Listing Model

  * Defined Mongoose schema for property listings (title, image, price, description, etc.).

* Database Initialization

  * Connected MongoDB database and added sample data.

* CRUD Routes for Listings

  * Index Route - View all listings
  * Show Route - View individual listing details
  * New & Create Routes - Add a new listing
  * Edit & Update Routes - Modify an existing listing
  * Delete Route - Remove a listing

### Part 2: UI Components & Styling

* Boilerplate Layout

  * Created a reusable boilerplate using `ejs-mate` for DRY templating.

* Navigation and Footer

  * Implemented a responsive navigation bar and footer for all pages.

* Page Styling

  * Styled the following pages using Bootstrap:

    * Index (All Listings)
    * New Listing Form
    * Edit Listing Form
    * Show Listing Page

### Part 3: Validation & Error Handling

* Client-Side Validation

  * Ensured forms cannot be submitted with empty or invalid inputs.

* Success & Failure Messages

  * Used flash messages to inform users of successful or failed operations.

* Robust Error Handling

  * Wrapped async routes with `wrapAsync` utility
  * Custom `ExpressError` class for better error descriptions
  * `error.ejs` page to display errors gracefully

* Joi Schema Validation

  * Added schema validation using Joi for server-side validation
  * Created middleware to centralize validation logic

## Getting Started

Clone the repository and run the project locally:

```bash
git clone https://github.com/your-username/wanderlust.git
cd wanderlust
npm install
npm start
```
Make sure MongoDB is running locally or provide a MongoDB Atlas connection string in `.env`.

## Technologies Used

* Node.js
* Express.js
* MongoDB & Mongoose
* EJS + ejs-mate
* Bootstrap 5
* Joi (for validation)

## Next Phase (Coming Soon)

In Phase Two, planned features include:

* User authentication (Register/Login)
* Flash messages and session handling
* Image uploads with Cloudinary
* Advanced filtering and search
