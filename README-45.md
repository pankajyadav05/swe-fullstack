# Game Development Task - 45 Minute Live Coding Round

## Objective

Create a simplified agent selection game using React.js, integrating with the Valorant API.

## Task Requirements (45 Minutes)

### **Front-End Development:**

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
   - OnClick, Add selected agent to history. Next redirect user to **Home Screen.**
   - Show visual distinction for selectable vs non-selectable agents

### **Rules:**

- Cannot select the same agent consecutively (if last game was Agent X, Agent X should be disabled)
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
   - Basic loading states
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

---

**Note:** Focus on working functionality over perfect design. A working app with basic styling is better than a beautiful app that doesn't work!
