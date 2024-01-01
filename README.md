# Game Agent Selection Screen Task

## Overview

This task involves creating a game agent selection screen where users can choose from a list of agents and start a game. The application will have specific rules (mentioned in task description) and state management requirements (using useContext only).

## Task Description

- Develop a game agent select screen using React.js.
- Fetch the list of agents from the Valorant API (https://valorant-api.com/v1/agents) through a Node.js back-end.
- The back-end should filter and send only the necessary fields to the front-end.
- Add a "Start Game" button on the home screen to navigate to the select agent screen.
- Implement functionality to select an agent and start the game.
- Display a "Game Started" screen upon selection.
- Implement specific rules for agent selection:
  - An agent cannot be selected in consecutive games.
  - An agent can be selected a maximum of 3 times.
  - A maximum of 10 games can be played. After that, show a "Limit Reached" screen.
  - Within the last 5 games (including the current one), no three agents should be the same.
- The user interface must clearly distinguish between selectable and non-selectable agents.
- Show a history of selected agents based on frequency of selection.

## Ground Rules

- Manage the state of selected agents using the useContext hook in React.
- The solution should be coded in JavaScript/TypeScript. Styling should be done in CSS or SCSS. Your choice.
- Put the code on your GitHub account in a private repo.
- **All Valorant API calling must be performed on backend side using Node.js.**
- You can add extra features or improvements. There will be bonus points for it.
- You can use other external libraries to speed up your work.
- You can use a styling framework (Material UI, Bootstrap, Tailwind, or other) for quick and consistent styling.
- If you're not able to implement all parts of the task, partial submissions are welcome.
- Provide the GitHub repository URL as a PRIVATE Git repository (also provide access) to prithvi@smartdino.tech and cc arun@smartdino.tech, hello@pankajyadav.dev
- The code should be properly organized and follow best practices for maintainability and scalability.
- Include a README with setup and run instructions.

## Evaluation rules

- Code Quality: Clean, well-organized, maintainable code.
- UI: Attention to details matters.
- Check full details about Evaluation criteria here [marks.md](MARKS.md)

### Good luck!
