# React Fetch CRUD Lab Implementation Plan

## Steps to Complete:

1. [x] Update App.js to manage questions state and fetch data on mount
2. [x] Update QuestionList.js to render QuestionItem components with props
3. [x] Update QuestionItem.js to handle delete and patch operations
4. [x] Update QuestionForm.js to handle form submission and POST new questions
5. [ ] Test the complete application

## Implementation Details:

### App.js
- ✅ Add useState for questions state
- ✅ Add useEffect to fetch questions from http://localhost:4000/questions
- ✅ Pass questions and handlers to child components

### QuestionList.js
- ✅ Receive questions as prop
- ✅ Map through questions to render QuestionItem components
- ✅ Pass delete and update handlers to QuestionItem

### QuestionItem.js
- ✅ Handle delete button click with DELETE request
- ✅ Handle correct answer dropdown change with PATCH request
- ✅ Call parent handlers to update state after API operations

### QuestionForm.js
- ✅ Handle form submission with POST request
- ✅ Format data correctly for API (prompt, answers array, correctIndex)
- ✅ Call parent handler to update state after successful POST

## Testing Instructions:
1. Run `npm run server` to start the JSON server
2. Run `npm start` to start the React application
3. Test all CRUD operations:
   - View questions (GET)
   - Add new questions (POST)
   - Delete questions (DELETE)
   - Update correct answers (PATCH)
