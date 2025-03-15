# 7GUI Tasks Implementation with SvelteKit

## Overview

This project implements the 7GUI tasks using SvelteKit, showcasing the expressiveness and capabilities of the Svelte framework in handling common GUI programming challenges. The 7GUI tasks serve as a benchmark for comparing different UI frameworks by implementing typical user interface scenarios.

## Project Description

The application is built with Aider and GPT-4o as an exercise in AI coding, demonstrating how AI can assist in developing complex user interfaces by automating repetitive tasks and providing intelligent suggestions.

## 7GUI Tasks

The project includes the following tasks, each representing a typical UI problem:

- **Counter**: Increment and decrement a counter value.
- **Temperature Converter**: Convert temperatures between Celsius and Fahrenheit.
- **Flight Booker**: Book a one-way or return flight with date selection.
- **Timer**: A countdown timer with start, stop, and reset functionality.
- **CRUD**: Create, Read, Update, and Delete entries in a list.
- **Circle Drawer**: Draw and manipulate circles on a canvas.
- **Cells**: A simple spreadsheet-like application.

## Technology Stack

- **Framework**: SvelteKit
- **Language**: JavaScript/TypeScript
- **Styling**: CSS/SCSS

## Goals

The primary goal of this project is to explore the strengths and weaknesses of SvelteKit in handling real-world UI challenges through the implementation of the 7GUI tasks.

For more information, visit the original [7GUI project page](https://eugenkiss.github.io/7guis/).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npx sv create

# create a new project in my-app
npx sv create my-app
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://svelte.dev/docs/kit/adapters) for your target environment.
