# General Specs

A general overview of the technology used on the project, how and why it's being used. 

## Tech Stack

The current selection of tools includes React + Next.js for the Frontend and NodeJS and Python for the Backend, data management will be done with DynamoDB and MariaDB.

### Frontend 
The frontend of the application has been built using React to be able to compose it using reusable components, and the main goal is to keep the business logic completely separated from the presentation layer, so the components here should have as little bussiness rules as possible.  All the processing and transformations must happen on the backend side.

### Backend
The data model is being split into the document handling section wich is related to candidates and campaigns, those are stored in DynamoDB since those are the structures that can change over time and will require more adaptation depending on the business needs.

For the components that require more structured data, we are using a regular relational database, in our case it's MariaDB.