# 7GUI Tasks Implementation with SvelteKit

## Project Overview
This project aims to implement the 7GUI tasks using SvelteKit to create a purely static website. The 7GUI tasks are a set of common GUI programming challenges designed to test the expressiveness of UI frameworks.

## Technology Stack
- **Framework**: SvelteKit
- **Language**: JavaScript/TypeScript
- **Styling**: CSS/SCSS

## 7GUI Tasks
1. **Counter**: A simple counter that can be incremented and decremented.
2. **Temperature Converter**: Convert temperatures between Celsius and Fahrenheit.
3. **Flight Booker**: Book a one-way or return flight.
4. **Timer**: A countdown timer with start, stop, and reset functionality.
5. **CRUD**: Create, Read, Update, and Delete operations on a list of items.
6. **Circle Drawer**: Draw and manipulate circles on a canvas.
7. **Cells**: A simple spreadsheet-like application.

## Component Structure
Each task will be implemented as a separate Svelte component. The components will be organized as follows:
- `src/routes/counter.svelte`
- `src/routes/temperature-converter.svelte`
- `src/routes/flight-booker.svelte`
- `src/routes/timer.svelte`
- `src/routes/crud.svelte`
- `src/routes/circle-drawer.svelte`
- `src/routes/cells.svelte`

## Routing
SvelteKit's file-based routing will be used to navigate between tasks. Each task will have its own route based on the component file name.

## State Management
State will be managed using Svelte's built-in reactivity. Each component will handle its own state, with props and events used for communication between components if necessary.

## Styling
Styling will be done using CSS or SCSS. Consider using a design framework like Tailwind CSS for consistent styling across components.

## Build and Deployment
The site will be built using SvelteKit's static site generation capabilities. Deployment can be done on platforms like Vercel or Netlify.

## Testing
Testing will be done using a combination of unit tests for individual components and end-to-end tests for the overall application. Consider using testing libraries like Jest and Cypress.

## Timeline and Milestones
- **Week 1**: Set up the project and implement the Counter and Temperature Converter tasks.
- **Week 2**: Implement the Flight Booker and Timer tasks.
- **Week 3**: Implement the CRUD and Circle Drawer tasks.
- **Week 4**: Implement the Cells task and conduct testing and deployment.
