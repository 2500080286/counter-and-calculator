COUNTER AND CALCULATOR  (React + Vite)
Question 7 - React State (useState)
=======================================

REQUIREMENT
-----------
Node.js version 18 or higher (check with:  node -v)

HOW TO RUN
----------
1. Extract the ZIP file.
2. Open a terminal / command prompt INSIDE the extracted folder
   (the folder that contains package.json).
3. Install the dependencies:

       npm install

4. Start the development server:

       npm run dev

5. Open the link shown in the terminal in your browser
   (normally  http://localhost:5173 ).

To stop the server press  Ctrl + C  in the terminal.

PROJECT STRUCTURE
-----------------
package.json     - project details and scripts
vite.config.js   - Vite configuration (React plugin)
index.html       - main HTML page (has the <div id="root">)
src/main.jsx     - entry point, renders <App /> into the root div
src/App.jsx      - Counter and Calculator components (useState)
src/style.css    - all CSS (responsive)

FEATURES
--------
Counter    : Increment, Decrement, Reset (state: count)
Calculator : +  -  x  /  with two number inputs and a Clear button
             Validation: message if a number is empty,
             and division by zero is blocked.

VIVA POINTS
-----------
- useState returns [value, setterFunction]. Calling the setter updates the
  value and React re-renders the component.
- Counter uses one state:  count.
- Calculator uses four states:  num1, num2, result, error.
- Inputs are "controlled": value comes from state, onChange updates state.
- Conditional rendering ({error !== "" && ...}) shows the error/result only
  when needed.
