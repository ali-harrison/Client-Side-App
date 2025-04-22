# DreamFest

DreamFest is a comprehensive application designed to manage a three-day music festival that includes a variety of events such as yoga, meditation, arts and crafts, healthy eateries, wellbeing workshops, and music performances. This project showcases my ability to implement database functions that allow festival organizers to efficiently manage locations and events.

## Project Overview

This application empowers festival organizers to add and manage locations and events. As plans evolve, the app supports adding, editing, and deleting events. While the UI and routes were pre-built, I was responsible for connecting them to the database by implementing necessary database functions.

## Setup

### Installation and Initialization

- Successfully cloned the repository and navigated into the directory.
- Installed all necessary packages and ran migrations and seeds to populate the database.
- Started the development server using `npm run dev`.

## Core Features and Implementations

### Displaying Locations and Events

1. **Displaying All Locations**:
   - Implemented the `getAllLocations` function to fetch and return all locations from the database, integrating it with the `GET /api/v1/locations` route.

2. **Displaying Events by Day**:
   - Developed the `getEventsByDay` function to retrieve events for a specific day, ensuring integration with the `GET /api/v1/schedule/:day` route.
   - Utilized SQL JOIN operations to combine relevant data from `events` and `locations` tables, filtering results by the specified day.

### Editing Locations

3. **Displaying the Edit Location Form**:
   - Implemented the `getLocationById` function to fetch data for a specific location, ensuring the form is pre-populated with current data.

4. **Submitting Location Edits**:
   - Integrated the "Edit Location" form with the server, using the `PATCH /api/v1/locations/:id` route to update location details in the database.

### Managing Events

5. **Adding New Events**:
   - Developed functionality to submit new events through the "Add New Event" form, utilizing the `POST /events` route.

6. **Deleting Events**:
   - Enabled event deletion via the `DELETE /api/v1/events/:id` route, ensuring efficient removal of events from the database.

## Stretch Goals and Enhancements

### Editing Events

- Implemented the `getEventById` function to support editing existing events, ensuring that forms are accurately populated with current event data.
- Enhanced the event update process through the `PATCH /events/:id` route.

### Adding and Deleting Locations

- Created components and routes to facilitate the addition and deletion of locations, ensuring seamless integration with existing application features.

### Testing and Quality Assurance

- Conducted tests on helper functions to ensure reliability and adherence to test-driven development principles.
- Optimized database queries to improve performance and reduce unnecessary data retrieval.

## Quality Measures and Optimization

- Improved site performance by optimizing images and ensuring efficient database queries.
- Enforced code consistency and readability through linting and formatting tools.
- Ensured separation of concerns by refactoring functions and maintaining single responsibility principles.
