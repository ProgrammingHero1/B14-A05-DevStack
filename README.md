# 🧱 A-5 Dev Stack Builder Website

## 📅 Deadlines
- 60 Marks: 13th September, 2026 (11:59 PM ⏱️)
- 50 Marks: No deadline for 50 marks.
- 30 Marks: Any time after the 60 marks window.

---

## 🚫 Key Rules
- Don't ask about mark distribution in the group. We don't provide it.
- Don't post assignment feedback after you receive it. If you face any problem or have any complaints, join a support session and discuss it.
- Don't use any lorem ipsum text, rather use relevant and meaningful text content.
- You can change the color if you want, but remember that it should not be a gobindo color.
- Use at least 8 git commits with meaningful messages.



---

## 🧩 Features & Requirements (50 Marks)

### 🧭 Navbar
- Navbar designed according to the UI.
- Left: brand logo + "Dev Stack" name.
- Center: nav links — Home, Technologies, Projects, About, Contact.
- Right: "Sign In" (text button) and "Sign Up" (filled pill button).
- Navbar stays sticky at the top while scrolling.

---

### 🍔 Mobile Navbar
- On small devices the navbar has three parts:
  - Left: hamburger menu icon
  - Center: brand logo
  - Right: Sign In and Sign Up buttons

![Hamburger menu](./ui/hamburger.png)

---

### 🎯 Banner / Hero
- Banner section includes:
  - Heading (two-tone: plain text + gradient text)
  - Description text
  - Two buttons — "Explore Technologies" (gradient) and "Learn More" (outlined)
  - Banner image

---

### 📦 JSON Data
Create 10-15 technology data with:
- id
- name
- category (Frontend / Backend / Database / Language / Styling / DevOps / Tools)
- description
- icon (image URL)
- rating (example: 4.8)
- difficulty (Beginner-Friendly / Intermediate / Advanced)
- badge (example: Popular, Fast, Essential, Containers)

**Example:**

```json
[
  {
    "id": "react",
    "name": "React",
    "category": "Frontend",
    "description": "A declarative, component-based JavaScript library for building modern user interfaces.",
    "icon": "https://icon.icepanel.io/Technology/svg/React.svg",
    "rating": 4.9,
    "difficulty": "Beginner-Friendly",
    "badge": "Popular"
  },
  {
    "id": "postgresql",
    "name": "PostgreSQL",
    "category": "Database",
    "description": "A powerful, open-source object-relational database system with proven reliability.",
    "icon": "https://icon.icepanel.io/Technology/svg/PostgresSQL.svg",
    "rating": 4.9,
    "difficulty": "Intermediate",
    "badge": "Top SQL"
  }
]
```

🚩 You can take help of AI Systems for generating the JSON Data.

🚩 Load the data from the JSON file — do not hardcode the array inside the component.

---

### 🃏 Technology Cards
- Display all technologies in a 3-column layout (responsive: 1 column on mobile, 2 on tablet).
- Each card includes:
  - Icon
  - Badge
  - Name
  - Description
  - Category chip
  - Difficulty
  - Rating with a star
  - "Add to Stack" button

---

### 🧰 Your Stack Section (Sidebar)
- A "Your Stack" panel sits beside the technology grid.
- Shows a heading and the selected count — example: "2 Technology Selected".
- By default the panel shows an empty message.

| Empty state | With selected items |
| --- | --- |
| ![Your Stack empty](./ui/YourStack-without.png) | ![Your Stack with items](./ui/YourStack-with.png) |

---

### ➕ Add to Stack Functionality
- Clicking "Add to Stack" adds that technology to the "Your Stack" panel.
- Each stack item shows: icon, name, category, and a remove (✕) button.
- Stack layout: 1 column.
- **The same technology cannot be added twice.** Trying again shows a warning alert.

- Once added, that card's button becomes disabled and reads "✓ Added to Stack".

---

### ❌ Remove Functionality
- Clicking the ✕ button on a stack item removes only that item from the stack.
- "Remove All" button clears the whole stack at once.

---

### 🦶 Footer
- Footer designed based on the UI.
- Brand block: logo, name, short description, social links (GitHub, Twitter, LinkedIn).
- Three link groups: Product, Company, Legal.
- Bottom bar: copyright text + Privacy and Terms links.

---

### 📱 Responsive Design
- Fully responsive across mobile, tablet, and desktop.
- Follow standard responsive practices.

---

# 🚀 Challenges Part (10 Marks)

### 🔔 Use a NPM Package React-Toastify
- Use react-toastify to show alerts for: add to stack, duplicate add attempt, remove, and remove all.

---

### ⏳ Loading State
- Show a loading message/spinner while the JSON data is being fetched.
- Note: since the JSON is a local file, the loading state may only be visible for a few milliseconds and can be hard to catch on screen. That is completely fine — the requirement is that the loading state exists and works, not that it stays visible for long.

---

### 🎨 Gradient Brand Theme
- Use one shared gradient (orange → pink → violet) for the brand name, hero heading highlight, and primary buttons.
- Define the gradient in one place so the whole UI can be re-themed by changing a single value.

---

### 📂 GitHub Repository
- Create a beautiful GitHub Readme with the following description:
  - Name of your project
  - A little description
  - Technology that you use
  - 3 features about your project

- Also answer these React questions at the end of your Readme (write the answers in your own words, short and simple):
  1. What is JSX, and why is it used in React?
  2. What is the difference between props and state?
  3. What does the `useState` hook do, and where did you use it in this project?
  4. What does the `useEffect` hook do, and why did you need it to load the JSON data?
  5. Why does every item in a `.map()` list need a unique `key` prop?
  6. What is conditional rendering? Show one place you used it (example: the empty stack message).
  7. How do you pass data from a parent component to a child component, and how does a child send something back to the parent?

---

## Optional Features:
1. Disable the "Add to Stack" button and change its label after a technology is added.
2. Keep the "Your Stack" panel sticky so it stays visible while scrolling the technology grid.
3. Show the selected count in the panel heading area and update it live.

---

## ⚙️ Technology You Can Use
- React.js
- Tailwind CSS, DaisyUI
- TypeScript / JavaScript (ES6+)
- React-Toastify (NPM Package)
- JSON (for technology data)
- Vite (build tool)

---

## ❓ Common FAQ

**1. Where can we deploy the site?**
Anywhere you like — Netlify, Vercel, Cloudflare Pages, or any other host. There is no fixed platform.

**2. Do we have to use TypeScript?**
No. You can use TypeScript or JavaScript. If you want to build the whole project in plain JavaScript, that is completely fine.

**3. Can we change the title, logo, and colors?**
Yes. The project title, logo, and color scheme are all yours to change — just keep them relevant to the project. Don't use random or gobindo colors and don't put an unrelated title/logo.

**4. Where do we get the technology logos/icons?**
You can use image URLs from Google or from anywhere you like. A good source with clean, ready-to-use tech logos is <https://techicons.dev/> — copy the icon URL from there and put it in your JSON data.

---

## 📤 What to submit:
- GitHub Repository Link:
- Live Site Link:
