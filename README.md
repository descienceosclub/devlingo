# DevLingo

DevLingo is a browser based, gamified introduction to HTML, CSS, JavaScript, and jQuery. It is designed for short practice sessions: read a mini lesson, edit the starter code, see the result, and complete a quick check.

## Try it

Open `index.html` in a modern browser, or visit the GitHub Pages link published for this repository. Choose a starting tier, enter a name if you like, and select a lesson on the path.

For the live preview and jQuery track, use an internet connection. The app itself has no server or database; it loads fonts, confetti, and jQuery from CDNs.

## What to expect

On first visit, DevLingo asks you to choose a level:

- **Entry** starts with HTML fundamentals.
- **Pro** starts with CSS.
- **Expert** starts with JavaScript.
- HTML and CSS lessons remain open for every tier, so students can return to fundamentals whenever they need to inspect a generated interface.

The learning path now has eight HTML lessons and eight CSS lessons, followed by JavaScript and jQuery practice. There is no fixed stopping point in the HTML/CSS path: learners can keep building the skills they need to inspect generated or vibe-coded pages.

| Track | Topics and expected outcomes |
| --- | --- |
| HTML Foundations (8 lessons) | Build page landmarks and nested content; choose semantic text; inspect links, media, forms, accessible labels, and control behavior. |
| Modern CSS (8 lessons) | Use selectors and the cascade, colors, spacing, readable type, Flexbox, responsive layouts, transitions, hover, and keyboard focus states. |
| Vanilla JavaScript | Declare values with `const` and `let`; select and update page elements; respond to clicks; use conditions and array iteration. |
| jQuery Speedrun | Select elements with `$()`; handle events; apply effects and styles; chain methods to update page content. |

### Example: CSS lesson 1

The **Selectors & Colors** lesson begins with a green button inside a lightly tinted hero area. After editing the starter code, the preview should show the change. For example, changing `.btn` or `#hero` colors changes the button or its surrounding section. Press **Run code** to check the lesson. A passing lesson shows a success message, awards 20 XP, and updates your saved path progress.

When a learner completes every lesson in a track, DevLingo awards a named badge and recognition message. If a check fails, the learner sees the expected output and an invitation to update the code and retry. Across the course, students build a set of working examples and practice inspecting, writing, and debugging front-end code.

## Progress and reset

Your name, tier, XP, hearts, streak, and completed lessons are stored in `localStorage` in the browser you use. They stay there until browser site data is cleared or you choose **Start fresh** at the bottom of the learning path. Progress does not sync to a teacher account, another browser, or another device. Each student gets a separate save in their own browser.

**Start fresh** asks for confirmation, then clears the saved DevLingo profile and returns to onboarding. It does not delete browser data for other sites.

## Share with students using GitHub

You can share this repository as source code, or publish it as a live website with GitHub Pages:

1. Create a GitHub repository and add `index.html`, `styles.css`, `app.js`, `lessons.js`, and this `README.md` at the repository root.
2. For a public classroom link, make the repository public. GitHub Pages publishes static files from a repository; this app needs no build command or backend.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, then select the `main` branch and `/ (root)` folder. Save the setting.
5. When Pages finishes publishing, copy the site URL from the Pages settings and share that URL with students. Share the repository URL too if you want them to read or download the source.

GitHub Pages publishes the site publicly, so only put material in the repository that you intend to make public. See the [GitHub Pages setup guide](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site) for current instructions.

## Project files

- `index.html` — app structure and dialogs
- `styles.css` — responsive design and dark theme
- `app.js` — navigation, preview sandbox, local progress, and rewards
- `lessons.js` — all current lesson definitions, starter code, hints, and checks

## Privacy and technical notes

- There is no account system, server, or external progress database.
- The lesson preview runs in a sandboxed iframe. Avoid entering personal or sensitive information into the editor.
- Google Fonts, canvas-confetti, and jQuery are loaded from third-party CDNs. The jQuery CDN is used only for jQuery lessons.
- The preview checks each lesson locally. It is a learning aid, not a production code security review.
