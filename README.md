# Game Development Task

## Objective

Create a game using React.js and Node.js, integrating with the Valorant API and DB.

## Task Requirements

1. **Back-End Development (Node.js):**

   - Fetch agent data from Valorant API (https://valorant-api.com/v1/agents).
   - Filter and group agents by role, sending only essential data to the front-end.

2. **Front-End Development (React.js):**

   - Implement a "Start Game" button on the home screen.
   - Develop a selection screen with these features:
     - Display a list of roles; selecting a role should filter agents accordingly.
     - Include an option to clear filters and show all agents.
     - Allow users to select an agent and lock in their choice with a "Lock In" button.
     - On clicking "Lock In", display a "Game Started" screen with the selected agent.
     - Distinguish between selectable and non-selectable agents visually.
     - Example screen layout: [SAMPLE SCREEN](https://mir-s3-cdn-cf.behance.net/project_modules/1400/94fe9596477133.5eaf7e1c3a48e.png)
   - "Game Started" screen:
     - Display the selected agent and a button to return to the home screen.
   - Home Screen Features:
     - Show history of selected agents in a table with agent icon and game start time.

3. **Agent Selection Rules:**

   - No consecutive game selection for the same agent.
   - Limit agent selection to 3 times.
   - Maximum of 10 games per user.
   - For the 5th game and onwards, if four different agents were chosen in the last four games, one of them must be selected for the current game.

4. **Data Management:**

   - Store selection history in the backend database [choose either MySQL, PostgreSQL or MongoDB].
   - You can use free DB hosting services like [Neon](https://neon.tech/), [PlanetScale](https://planetscale.com/), [MongoDB](https://www.mongodb.com/).
   - Use the useContext hook in React for state management.

5. **Additional Requirements:**
   - Code in JavaScript/TypeScript, style in CSS/SCSS.
   - Organize the code in a private GitHub repository. Grant access to prithvi@gitforcetalent.com, cc roshan@gitforcetalent.com, pankaj@gitforcetalent.com
   - Incorporate a README with setup and run instructions.
   - Valorant API calls should be exclusively backend-based.
   - Use of external libraries and styling frameworks (e.g., Material UI, Bootstrap, Tailwind) is allowed.

## Submission

Provide the GitHub repository URL as a PRIVATE Git repository and grant access to the specified emails.

## Evaluation

Evaluation will be based on code quality, user interface design, and adherence to the task requirements. For detailed evaluation criteria, refer to [marks.md](MARKS.md).

### Best of luck!
