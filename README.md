markdown
# 📘 ReactJS Notes

## 🚀 Why React is Popular
- Fast rendering using **Virtual DOM**
- **Reusable Components** for modular development
- Easy to learn (if you know JavaScript)
- Strong community support
- Trusted by big companies like **Netflix** and **Instagram**

---

## 🖥️ 1. Single Page Application (SPA)
A **Single Page Application** loads only one HTML page and dynamically updates content without refreshing the page.

**Examples:** Gmail, Facebook  
👉 The page does not reload completely – only data updates.

---

## ⚡ 2. Virtual DOM
**DOM = Document Object Model**

The **Virtual DOM** is a lightweight copy of the Real DOM created and managed by React.

**How it works:**
1. User interacts (click, input, etc.)
2. State changes
3. React creates a new Virtual DOM
4. React compares old Virtual DOM with new Virtual DOM
5. React updates only changed parts in Real DOM

This comparison process is called the **Diffing Algorithm**.

### 🔍 Real DOM vs Virtual DOM

| Feature       | Real DOM              | Virtual DOM              |
|---------------|-----------------------|--------------------------|
| Speed         | Slow                  | Fast                     |
| Update        | Updates entire tree   | Updates only changed parts |
| Memory        | Heavy                 | Lightweight              |
| Efficiency    | Less                  | More                     |

---

## 📝 3. JSX (JavaScript XML)
JSX is a **syntax extension** for JavaScript used in React.  
It allows writing **HTML-like structure inside JavaScript code**.

**Example:**
```javascript
const element = <h1>Hello React</h1>;
✅ Rules of JSX
Must return a single parent element (use Fragment <> </> or <div>)

Close all tags (<img src="image.jpg" />)

Use className instead of class

Use CamelCase for attributes (e.g., onClick, onChange, backgroundColor)

🔗 Embedding JavaScript in JSX
Wrap JavaScript expressions in { }.

Examples:

javascript
const name = "TKA";
return <h1>Hello {name}</h1>;

<h1>{5 + 5}</h1>
🎯 Handling Events
javascript
<button onClick={handleClick}>Click</button>
📊 Comparison: HTML vs JSX
Feature	HTML	JSX
class	class	className
Attributes	lowercase	camelCase
Multiple elements	Allowed	Must wrap in Fragment/div
Self-closing	Optional	Required ( )


🔄 4. Unidirectional Data Flow
Data flows only one way: Parent → Child

Achieved using props

Restriction: Data does not automatically flow from child to parent

📦 5. npm (Node Package Manager)
npm is the default package manager for Node.js.

It is used to:

Install libraries

Manage dependencies

Run scripts

Create React projects

Note: npm comes automatically with Node.js.

Update npm:

bash
npm install -g npm
⚡ 6. Create React App Using Vite
Vite is fast and lightweight compared to older setups.

Steps:

bash
npm create vite@latest my-react-app
npm run dev
🛠️ Getting Started
Install Node.js (npm comes bundled with it).

Verify installation:

bash
node -v
npm -v
Create a new React project using Vite:

bash
npm create vite@latest my-react-app
cd my-react-app
npm install
npm run dev
Open http://localhost:5173 in your browser to see your app running.