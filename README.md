# The Complete Full-Stack Web Development Bootcamp Report

## Section 9: Flexbox

## 54. Display: Flex
Purpose: activate Flexbox.

`display: flex;` turns the parent element into a **flex container**, and its children become **flex items**.

Default behavior:
- Items are laid out in a horizontal row
- Items do not wrap onto a new line
- Item size depends on content

Flexbox is best suited for **one-dimensional layouts** (row or column).

## 55. Flex Direction
Defines the direction in which flex items are laid out.

Values:
- `row` (default): left to right
- `row-reverse`: right to left
- `column`: top to bottom
- `column-reverse`: bottom to top

This property defines the **main axis** and directly affects `justify-content`.

## 56. Flex Layout (Alignment & Wrapping)

### Main Axis
Use `justify-content`:
- `flex-start`
- `center`
- `space-between`
- `space-around`
- `space-evenly`

### Cross Axis
Use `align-items`:
- `stretch` (default)
- `center`
- `flex-start`
- `flex-end`

### Wrapping
Use `flex-wrap`:
- `nowrap`
- `wrap`
- `wrap-reverse`

### Multiple Lines
Use `align-content`:
- `flex-start`
- `center`
- `space-between`
- `space-around`

## 57. Flex Sizing
Controls the size of flex items.

Properties:
- `flex-grow`
- `flex-shrink`
- `flex-basis`

Shorthand syntax:
`flex: grow shrink basis;`

Examples:
- `flex: 1;`
- `flex: 0 0 200px;`

## Summary
- Flexbox is used for one-dimensional layouts
- It provides easy alignment and spacing
- Items can grow and shrink flexibly
- Commonly used for navbars, cards, forms, and button groups

## Section 10: Grid

## 60. Display: Grid
Purpose: activate CSS Grid layout.

`display: grid;` turns the parent element into a **grid container**, and its children become **grid items**.

Key characteristics:
- Grid works in **two dimensions** (rows and columns)
- Layout is defined explicitly
- More control than Flexbox for complex layouts

Grid is best suited for **page-level layouts** and complex structures.

## 61. Grid Sizing
Defines the size of rows and columns.

### Columns
Use `grid-template-columns`:
- Fixed units: `px`, `%`
- Flexible units: `fr`
- Automatic sizing: `auto`

Example values:
- `grid-template-columns: 200px 1fr 1fr;`
- `grid-template-columns: repeat(3, 1fr);`

### Rows
Use `grid-template-rows`:
- Same sizing options as columns

Special functions:
- `minmax(min, max)`
- `repeat()`
- `auto-fit` / `auto-fill`

Grid sizing allows layouts to be **responsive without media queries**.

## 62. Grid Placement
Controls where grid items are positioned inside the grid.

### Line-based placement
- `grid-column-start`
- `grid-column-end`
- `grid-row-start`
- `grid-row-end`

Shorthand:
- `grid-column: start / end;`
- `grid-row: start / end;`

### Span-based placement
- `grid-column: span 2;`
- `grid-row: span 3;`

### Named areas
Define layout using `grid-template-areas` and assign items with `grid-area`.

Grid placement provides **precise control** over item positioning.

## Summary
- CSS Grid is designed for two-dimensional layouts
- Ideal for overall page structure
- Provides precise control over rows and columns
- Complements Flexbox rather than replacing it

## Section 16: The Document Object Model (DOM)

## 114. Adding JavaScript to Websites
JavaScript can be added to a website in three main ways:
- Inline JavaScript (not recommended)
- Internal JavaScript using `<script>` tags
- External JavaScript using a separate `.js` file (best practice)

JavaScript is usually loaded at the end of the HTML body or with `defer` to ensure the DOM is fully loaded before execution.

## 115. Introduction to the Document Object Model (DOM)
The DOM represents the HTML document as a **tree structure** of objects.

Key points:
- The browser converts HTML into the DOM
- Each HTML element becomes a node
- JavaScript can access and modify the DOM dynamically

The DOM acts as the bridge between HTML and JavaScript.

## 116. Solution to the DOM Challenge
This section focuses on applying DOM concepts to solve a practical problem.

Key takeaways:
- Use DOM selection methods to target elements
- Apply changes using JavaScript logic
- Reinforces understanding of DOM manipulation workflow

## 117. Selecting HTML Elements with JavaScript
Common methods to select elements:

- `document.getElementById()`
- `document.getElementsByClassName()`
- `document.getElementsByTagName()`
- `document.querySelector()`
- `document.querySelectorAll()`

`querySelector` and `querySelectorAll` are the most flexible and commonly used methods.

## 118. Manipulating and Changing Styles of HTML Elements with JavaScript
JavaScript can change CSS styles dynamically using the `style` property.

Examples of manipulation:
- Changing colors, fonts, spacing
- Showing or hiding elements
- Creating visual feedback for user interaction

Inline styles set by JavaScript override external CSS.

## 119. Separation of Concerns: Structure vs Style vs Behaviour
Web development follows the principle of separation of concerns:
- HTML handles structure
- CSS handles style
- JavaScript handles behavior

This approach improves:
- Maintainability
- Readability
- Scalability of code

JavaScript should not replace CSS but enhance interactivity.

## 120. Text Manipulation and the Text Content Property
JavaScript can modify text inside elements.

Key properties:
- `textContent`: changes only text
- `innerHTML`: changes HTML structure and content

`textContent` is safer and faster when working with plain text.

## 121. Manipulating HTML Element Attributes
JavaScript can access and modify element attributes.

Common methods:
- `getAttribute()`
- `setAttribute()`
- `removeAttribute()`

This is often used for:
- Changing image sources
- Updating links
- Toggling classes or states

## Summary
- The DOM allows JavaScript to interact with HTML dynamically
- Elements can be selected, styled, and modified
- Clear separation of HTML, CSS, and JavaScript is essential
- DOM manipulation is fundamental to interactive web applications

## Section 17: JavaScript Event Listeners, Functions, and Objects
(Project lessons skipped)

## 136. Adding Event Listeners to a Button
JavaScript responds to user interactions using **event listeners**.

Key points:
- Use `addEventListener()` to listen for events
- Common events: `click`, `mouseover`, `keydown`
- Keeps JavaScript separate from HTML

Event listeners allow interactive and dynamic behavior on websites.

## 137. Higher Order Functions and Passing Functions as Arguments
A **higher-order function** is a function that:
- Takes another function as an argument, or
- Returns a function

JavaScript treats functions as **first-class citizens**, meaning they can be passed around like variables.

This concept is fundamental for:
- Callbacks
- Event handling
- Functional programming patterns

## 138. Higher Order Function Challenge Solution
This lesson reinforces:
- Passing functions as arguments
- Executing callbacks inside other functions
- Understanding function flow and execution order

It strengthens confidence in using higher-order functions correctly.

## 139. How to Play Sounds on a Website
JavaScript can control audio using the `Audio` object.

Key ideas:
- Create sound effects dynamically
- Trigger sounds based on user actions
- Enhance user experience with audio feedback

Audio is often combined with event listeners.

## 140. How to Use Switch Statements in JavaScript
The `switch` statement is used for multiple conditional branches.

Key points:
- Cleaner alternative to long `if...else` chains
- Uses `case`, `break`, and `default`
- Commonly used with user input and key presses

Switch statements improve readability in multi-condition logic.

## 141. A Deeper Understanding of JavaScript Objects
Objects store related data and behavior together.

Key concepts:
- Objects consist of properties and methods
- Data is stored as key-value pairs
- Objects model real-world entities in code

Objects are a core building block of JavaScript.

## 142. Objects, Their Methods, and the Dot Notation
Dot notation is used to:
- Access object properties
- Call object methods

Understanding dot notation is essential for:
- DOM manipulation
- Working with APIs
- Structuring complex applications

## 144. Using Keyboard Event Listeners to Check for Key Presses
JavaScript can detect keyboard input using events like:
- `keydown`
- `keyup`

Key uses:
- Games and interactive apps
- Accessibility features
- Shortcut keys

Keyboard events expand interaction beyond mouse clicks.

## 145. Understanding Callbacks and How to Respond to Events
Callbacks are functions executed after an event occurs.

Key ideas:
- Event-driven programming
- Asynchronous behavior
- Non-blocking execution

Callbacks are heavily used in:
- Event listeners
- Timers
- API requests

## 146. Adding Animation to Websites
JavaScript can add animation by:
- Modifying CSS classes
- Changing styles dynamically
- Using timing functions

Animations improve:
- User engagement
- Visual feedback
- Overall user experience

## Summary
- Event listeners enable user interaction
- Higher-order functions and callbacks are core JavaScript concepts
- Objects organize data and behavior
- Keyboard events and animations enhance interactivity

## Section 24: Express.js with Node.js
(Project lessons skipped)

## 201. What Is Express?
Express is a **minimal and flexible Node.js web framework**.

Key points:
- Built on top of Node.js
- Simplifies server-side development
- Used to build APIs and web applications
- Handles routing, requests, and responses

Express is widely used in backend development.

## 202. Creating Our First Server with Express
An Express server is created by:
- Importing the Express module
- Initializing an app instance
- Defining routes
- Starting a server with a listening port

Express makes server setup faster and cleaner than using Node.js alone.

## 203. HTTP Requests
Express handles different HTTP methods:

- `GET`: retrieve data
- `POST`: send data
- `PUT`: update data
- `DELETE`: remove data

Key concepts:
- Request (`req`)
- Response (`res`)
- Route paths

Understanding HTTP requests is essential for RESTful APIs.

## 204. Postman
Postman is a tool for testing APIs.

Used to:
- Send HTTP requests
- Test API endpoints
- Inspect responses
- Debug backend logic

Postman is essential when developing and testing servers.

## 205. Introduction to Middlewares
Middleware functions sit **between the request and the response**.

They can:
- Modify request and response objects
- Execute code
- End the request-response cycle
- Call the next middleware

Middlewares are a core concept in Express.

## 206. Custom Middlewares
Custom middleware functions are user-defined.

Common use cases:
- Logging requests
- Authentication checks
- Data validation
- Error handling

Custom middlewares increase code reusability and organization.

## Summary
- Express simplifies backend development with Node.js
- Routes handle HTTP requests
- Postman is used for API testing
- Middlewares control request flow and logic

## Section 25: EJS

## 209. What Is EJS?
EJS (Embedded JavaScript) is a **templating engine** for Node.js.

Key points:
- Allows embedding JavaScript into HTML
- Used with Express to generate dynamic web pages
- Separates logic from presentation

EJS makes it easy to render dynamic content on the server.

## 210. EJS Tags
EJS uses special tags to embed JavaScript.

Common tags:
- `<% %>`: execute JavaScript
- `<%= %>`: output escaped content
- `<%- %>`: output unescaped HTML

Choosing the correct tag is important for security and rendering.

## 211. Passing Data to EJS Templates
Data is passed from Express to EJS using the `render()` method.

Key ideas:
- Pass variables as an object
- Access variables directly in EJS files
- Enables dynamic content rendering

This allows pages to change based on server-side data.

## 212. EJS Partials and Layouts
Partials are reusable template components.

Used for:
- Headers
- Footers
- Navigation bars

Layouts help:
- Maintain consistent structure
- Reduce code duplication
- Improve maintainability

## Summary
- EJS is used to generate dynamic HTML on the server
- Tags control logic and output
- Data can be passed easily from Express
- Partials and layouts improve code reuse and structure

## Section 28: Application Programming Interfaces (APIs)

## 225. Introduction to APIs
An API (Application Programming Interface) allows different software systems to **communicate with each other**.

Key ideas:
- Acts as a bridge between applications
- Enables data exchange and functionality sharing
- Commonly used in web and mobile applications

APIs are essential for modern web development.

## 226. Structuring API Requests
API requests follow a structured format.

Key components:
- Endpoint (URL)
- HTTP method (GET, POST, PUT, DELETE)
- Headers
- Parameters (query or path)
- Body (for POST/PUT requests)

Well-structured requests ensure reliable communication with APIs.

## 227. What Is JSON?
JSON (JavaScript Object Notation) is a lightweight data format.

Characteristics:
- Human-readable
- Easy for machines to parse
- Uses key-value pairs
- Language-independent

JSON is the most common format for API data exchange.

## 228. Making Server-Side API Requests with Axios
Axios is a popular library for making HTTP requests.

Key points:
- Works on both client and server
- Supports promises and async/await
- Simplifies request and response handling

Axios is widely used in Express applications for consuming APIs.

## 229. API Authentication
API authentication ensures secure access to resources.

Common methods:
- API keys
- Basic authentication
- Bearer tokens
- OAuth

Authentication prevents unauthorized access and protects data.

## 230. REST APIs
REST (Representational State Transfer) is an API design style.

Core principles:
- Stateless communication
- Resource-based URLs
- Standard HTTP methods
- Consistent responses

REST APIs are scalable, predictable, and widely adopted.

## Summary
- APIs enable communication between systems
- JSON is the standard data format
- Axios simplifies API requests
- Authentication secures APIs
- REST defines best practices for API design

## Section 35: Authentication and Security – Handling Credentials & Designing a Secure App
(Project lessons skipped)

## 266. Introduction to Authentication
Authentication verifies the **identity of users**.

Key concepts:
- Confirms who the user is
- Different from authorization (what users can do)
- Essential for secure applications

Authentication is the foundation of web security.

## 267. Level 1: Registering Users with Email and Password
Basic authentication using:
- User registration forms
- Email and password storage

Key ideas:
- Store user credentials securely
- Never store passwords in plain text
- Validate user input

This is the starting point of authentication systems.

## 268. Level 2: Encryption and Hashing
Passwords should be **hashed**, not encrypted.

Key points:
- Hashing is one-way
- Encryption is reversible
- Hash functions protect passwords even if the database is compromised

Hashing is essential for password security.

## 269. How to Hack Passwords
This lesson explains common attack methods to promote awareness.

Key topics:
- Brute force attacks
- Dictionary attacks
- Rainbow tables

Understanding attacks helps developers design stronger defenses.

## 270. Level 3: Salting Passwords for Improved Encryption
Salting adds random data to passwords before hashing.

Benefits:
- Prevents rainbow table attacks
- Makes hashes unique
- Increases overall security

Salting is a standard practice in secure authentication.

## 271. Managing Cookies and Sessions
Sessions allow servers to remember users.

Key concepts:
- Cookies store session IDs
- Sessions maintain login state
- Helps manage authentication across requests

Sessions enable persistent user experiences.

## 272. Level 5: Hide Your Secrets with Environment Variables
Sensitive information should not be hard-coded.

Use environment variables for:
- API keys
- Database credentials
- OAuth secrets

This improves security and deployment flexibility.

## 273. Set Up Your Google OAuth Credentials
OAuth allows third-party authentication.

Key ideas:
- Use Google as an identity provider
- Configure client ID and secret
- Secure user login without handling passwords directly

OAuth improves security and user convenience.

## 274. Level 6: OAuth – Implement “Sign In with Google”
OAuth implementation steps:
- Redirect users to Google
- Handle authentication callbacks
- Create or find users in the database

This enables secure, passwordless authentication.

## 275. Finish the App: Let Users Submit Secrets
Final integration of authentication features.

Key outcomes:
- Only authenticated users can access protected features
- Users can securely submit and view content
- Demonstrates a complete authentication flow

## Summary
- Authentication protects user identity
- Hashing and salting secure passwords
- Sessions manage login state
- Environment variables protect secrets
- OAuth enables secure third-party authentication

