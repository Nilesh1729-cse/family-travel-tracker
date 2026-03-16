# Family Travel Tracker

A web application to track visited countries for multiple users, built with Node.js, Express, PostgreSQL, and EJS.

## Features

- User selection with color-coded tracking
- Add countries to a user's visited list
- Interactive world map showing visited countries in user colors
- Database storage with PostgreSQL

## Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: PostgreSQL
- **Frontend**: EJS templates, CSS, JavaScript
- **Other**: Body-parser, Static file serving

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd family-travel-tracker
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up PostgreSQL database:
   - Create a database named `world`
   - Run the SQL queries in `queries.sql` to create tables and insert initial data

4. Start the server:
   ```bash
   npm start
   # or for development
   nodemon index.js
   ```

5. Open your browser to `http://localhost:3000`

## Usage

- Select a user from the dropdown
- Enter a country name and click "Add Country"
- View the updated map with visited countries highlighted in the user's color

## Database Schema

- `users`: Stores user information (id, name, color)
- `visited_countries`: Stores visited countries per user (id, country_code, user_id)
