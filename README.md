# Conference Event Planner Docs

## Overview
React app with Redux Toolkit for state management. Plans conference events: select venues (rooms, capacities, costs), with placeholders for AV add-ons and meals. Uses Vite for builds. Repo: "conference_event_planner"; package: "eventone". Based on coding template.

**Key Features:**
- Venue selection with quantities (e.g., max 3 for Auditorium Hall).
- Total cost display.
- Basic landing page.
- Static "About Us" page (not fully integrated).

**Tech:**
- JavaScript/React
- Redux Toolkit
- Vite

## Installation
**Prerequisites:** Node.js 18+, npm.

1. `git clone https://github.com/QuestScrolls/conference_event_planner.git`
2. `cd conference_event_planner`
3. `npm install`

## Running
- Dev: `npm run dev` (localhost:5173)
- Build: `npm run build`
- Preview: `npm run preview`
- Lint: `npm run lint`

## Structure
```
public/  # Assets (images)
src/
├── assets/  # React logo
├── AboutUs.jsx  # Static about
├── App.jsx  # Landing
├── ConferenceEvent.jsx  # Planning UI
├── TotalCost.jsx  # Cost summary
├── {av,meals,venue}Slice.js  # Redux slices
├── store.js  # Redux store
├── main.jsx  # Entry
└── *.css  # Styles
Other: .eslintrc.cjs, index.html, package.json, vite.config.js
```

## Dependencies
| Runtime | Version | Purpose |
|---------|---------|---------|
| @reduxjs/toolkit | ^2.2.3 | State mgmt |
| react | ^18.2.0 | Core |
| react-dom | ^18.2.0 | DOM |
| react-redux | ^9.1.1 | Bindings |

| Dev | Version | Purpose |
|-----|---------|---------|
| @types/react* | ^18.2.* | Types |
| @vitejs/plugin-react | ^4.2.1 | Vite React |
| eslint* | ^8/7.* | Linting |
| vite | ^5.2.0 | Build |

## Redux
- **Store:** Includes venue reducer (AV/meals defined but not added).
- **Venue Slice:** Venues array; reducers: increment/decrement quantity (limits apply).
- **AV/Meals Slices:** Placeholders (empty reducers).

## Components
- **App.jsx:** Welcome + "Get Started" button.
- **ConferenceEvent.jsx:** Venue/add-ons/meals sections; quantity controls.
- **TotalCost.jsx:** Displays totals (incomplete).
- **AboutUs.jsx:** Company info.
- **main.jsx:** Renders App with Redux Provider.

## Usage
1. Run dev server.
2. Select venues, adjust quantities.
3. View totals (add-ons/meals non-functional).

## Improvements
- Add AV/meals to store/logic.
- Implement routing.
- Enhance UX/validation.
