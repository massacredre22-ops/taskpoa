# TaskPoa 🌱

**Learn · Complete · Grow**

A simple, client-side learning project that explores a legitimate **tasks and rewards** experience.

> **Demo only.** Points have no cash value and cannot be withdrawn.  
> This is **not** a live rewards service. No deposits or payments are required.

---

## What it is

TaskPoa is a single-page demo that lets users:

- Create a local profile (display name + username)
- Complete short learning tasks
- Earn **demo points** that are stored only in the browser
- Track progress on a personal dashboard

Everything runs in the browser. There is no backend, no accounts server, and no real money.

---

## Features

| Feature | Description |
|--------|-------------|
| **Local profile** | Display name + username saved in `localStorage` |
| **Demo points** | Start with 200 pts. Each completed task awards +10 |
| **3 tasks** | Quiz, Learning task, Growth reflection |
| **Progress tracking** | Dashboard + progress pill update live |
| **Reset** | One-click reset of points & tasks (profile is kept) |
| **Responsive UI** | Works on mobile and desktop |
| **Accessible** | Labels, focus styles, `aria-live` messages |

### The three tasks

1. **Quick Quiz** – Answer: capital of Kenya (Nairobi)
2. **Learning Task** – One-click complete
3. **Growth Reflection** – Write a short skill/habit goal (≥ 5 characters)

Maximum demo balance: **230 points**.

---

## How to run

### Option 1 – Open directly
1. Download or clone the repo
2. Open `index.html` in any modern browser

### Option 2 – Local server (recommended)
```bash
# From the project folder
python -m http.server 8080
# or
npx serve .
```
Then visit `http://localhost:8080`

No build step or dependencies required.

---

## Technical notes

- **Stack**: Pure HTML + CSS + vanilla JavaScript
- **Storage**:
  - `taskpoa_demo_v2` – points and task completion
  - `taskpoa_profile_v1` – display name and username
- **Integrity check**: On load, the app verifies that points match the number of completed tasks. Tampered values are discarded and the demo resets to the default state.
- **No network calls**: Fully offline after the page is loaded.

---

## Project structure

```
taskpoa/
├── index.html      # Complete demo (HTML + CSS + JS)
└── README.md
```

---

## Roadmap / learning goals

This project is intentionally small so it can be used to practice:

- Semantic HTML and accessible forms
- CSS custom properties and responsive layouts
- Client-side state with `localStorage`
- Progressive enhancement of a simple task flow
- Clear “demo only” messaging for legitimacy

Possible future experiments (not implemented):

- More task types
- Simple server-side persistence
- User authentication
- Real (non-cash) reward systems with clear rules

---

## Disclaimer

TaskPoa is a **learning / portfolio project**.

- Points are fictional and have **no monetary value**
- Nothing can be withdrawn or exchanged for cash
- No user data is sent to any server
- The authors are not operating a rewards or money-making platform

If you are looking for a production tasks-and-rewards product, this is not it.

---

## License

This project is provided for educational purposes.  
Feel free to fork, study, and improve it.

---

**Motto:** *Better skills. Brighter tomorrows.*
