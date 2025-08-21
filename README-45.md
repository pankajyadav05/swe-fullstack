# Game Development Task - 45 Minute Live Coding Round

## Objective

Create a simplified agent selection game using React.js, integrating with the Valorant API.

## Task Requirements (45 Minutes)

### **Front-End Development (React.js Only):**

1. **Home Screen:**

   - Display a "Start Game" button
   - Show a simple list of previously selected agents (stored in local state/localStorage)

2. **Agent Selection Screen:**

   - Fetch agent data directly from Valorant API (https://valorant-api.com/v1/agents) in the frontend
   - Display agents in a grid/list format with:
     - Agent portrait/icon
     - Agent name
     - Role badge
   - Include a role filter dropdown (Duelist, Controller, Initiator, Sentinel, All)
   - Allow user to select an agent and click "Lock In"
   - Show visual distinction for selectable vs non-selectable agents

3. **Game Started Screen:**
   - Display selected agent details (name, portrait, role)
   - Show "Back to Home" button
   - Add selected agent to history

### **Simplified Rules:**

- **Only 1 rule**: Cannot select the same agent consecutively (if last game was Agent X, Agent X should be disabled)
- Maximum 5 games total (after 5 games, show "Game limit reached" message)

### **Technical Requirements:**

1. **State Management:**

   - Use React hooks (useState, useEffect)
   - Store game history in localStorage (no backend needed)
   - Use React Context for global state (optional - can use prop drilling if faster)

2. **Data Structure for History:**

   ```javascript
   {
     games: [
       {
         id: 1,
         agentName: "Jett",
         agentIcon: "url",
         timestamp: "2024-01-01T10:00:00Z",
       },
     ];
   }
   ```

3. **API Integration:**

   - Make direct API calls from React components
   - Handle loading states
   - Basic error handling

4. **Styling:**
   - Use any CSS framework (Tailwind, Bootstrap, or plain CSS)
   - Focus on functionality over perfect design
   - Responsive design not required

### **Deliverables (End of 45 Minutes):**

1. **Working React Application** with:

   - Home screen with game history
   - Agent selection with role filtering
   - Game started screen
   - Navigation between screens

2. **Core Functionality:**

   - API data fetching and display
   - Agent selection with basic rule enforcement
   - Local storage persistence
   - Screen transitions

3. **Code Quality:**
   - Clean, readable code
   - Proper component structure
   - Basic error handling

## **Evaluation Focus:**

1. **Functionality (40 points):**

   - API integration works
   - Agent selection and filtering
   - Navigation between screens
   - Rule enforcement (consecutive agent prevention)

2. **Code Quality (30 points):**

   - Component organization
   - State management approach
   - Code readability

3. **User Experience (20 points):**

   - Intuitive interface
   - Loading states
   - Visual feedback

4. **Problem Solving (10 points):**
   - Approach to challenges
   - Debugging skills
   - Time management

## **Setup Instructions:**

```bash
# Quick start
npx create-react-app valorant-game
cd valorant-game
npm start
```

## **API Reference:**

- **Agents Endpoint:** `https://valorant-api.com/v1/agents`
- **Response includes:** uuid, displayName, displayIcon, role.displayName

## **Time Management Suggestions:**

- **0-10 min:** Project setup, API exploration, basic component structure
- **10-25 min:** Agent fetching, display, and role filtering
- **25-35 min:** Selection logic, rule enforcement, navigation
- **35-45 min:** History storage, polish, testing

## **Bonus (if time permits):**

- Add loading spinners
- Improve visual design
- Add agent abilities display
- Smooth transitions between screens

---

**Note:** Focus on working functionality over perfect design. A working app with basic styling is better than a beautiful app that doesn't work!
