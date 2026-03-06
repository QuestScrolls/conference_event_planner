Conference Event Planner Documentation
Overview
This is a React application built with Redux Toolkit for state management, designed to help users plan and calculate costs for conference events. The app allows selection of venues (rooms with capacities and costs), with plans for add-ons (AV equipment) and meals, though those sections are currently placeholders with empty reducer logic. It uses Vite as the build tool for fast development and production builds.
The project name in package.json is "eventone", but the repository is named "conference_event_planner". It appears to be based on a coding project template, as indicated in the original README.
Key features:

Select and quantify venues for the event.
Quantity limits (e.g., max 3 for Auditorium Hall).
Display total costs.
Basic landing page with navigation to planning sections.
Static "About Us" page (though not integrated in the provided code).

Languages and frameworks:

JavaScript (React)
State management: Redux Toolkit
Build tool: Vite

Installation
Prerequisites

Node.js (version 18 or higher recommended)
npm (comes with Node.js)

Steps

Clone the repository:textgit clone https://github.com/QuestScrolls/conference_event_planner.git
Navigate to the project directory:textcd conference_event_planner
Install dependencies:textnpm installThis will install all required packages based on package.json, including React, Redux Toolkit, and development tools like ESLint and Vite.

Running the Application
Development Mode
Run the app in development mode with hot reloading:
textnpm run dev
Open http://localhost:5173 in your browser.
Build for Production
Build the optimized production version:
textnpm run build
Preview Production Build
Preview the built app locally:
textnpm run preview
Linting
Check code for linting issues:
textnpm run lint
