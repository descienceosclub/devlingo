# DevLingo

DevLingo is a browser based, gamified introduction to HTML, CSS, JavaScript, and jQuery. It is designed for short practice sessions: read a mini lesson, edit the starter code, see the result, and complete a quick check.

## Try it

Open `index.html` in a modern browser, or visit the GitHub Pages link published for this repository. Choose a starting tier, enter a name if you like, and select a lesson on the path.

For the live preview and jQuery track, use an internet connection. The app itself has no server or database; it loads fonts, confetti, and jQuery from CDNs.

## What to expect

On first visit, DevLingo asks you to choose a level:

- **Entry** starts at Level 1 with HTML fundamentals.
- **Pro** starts at Level 6 with CSS and layout practice.
- **Expert** starts at Level 12 with advanced JavaScript concepts.

The learning path contains four tracks with four lessons each:

| Track | Topics and expected outcomes |
| --- | --- |
| HTML Foundations | Build a page skeleton; choose semantic text elements; add links and images with useful attributes; make a form with an input and button. |
| Modern CSS | Target classes and IDs; use color; explain the box model; arrange items with Flexbox; add hover states and transitions. |
| Vanilla JavaScript | Declare values with `const` and `let`; select and update page elements; respond to clicks; use conditions and array iteration. |
| jQuery Speedrun | Select elements with `$()`; handle events; apply effects and styles; chain methods to update page content. |

### Example: CSS lesson 1

The **Selectors & Colors** lesson begins with a green button inside a lightly tinted hero area. After editing the starter code, the preview should show the change. For example, changing `.btn` or `#hero` colors changes the button or its surrounding section. Press **Run code** to check the lesson. A passing lesson shows a success message, awards 20 XP, and updates your saved path progress.

Across the full course, students should finish with a small portfolio of working examples and practice reading, writing, and debugging common front-end code.

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
- `lessons.js` — all 16 lessons, starter code, hints, and checks

## Privacy and technical notes

- There is no account system, server, or external progress database.
- The lesson preview runs in a sandboxed iframe. Avoid entering personal or sensitive information into the editor.
- Google Fonts, canvas-confetti, and jQuery are loaded from third-party CDNs. The jQuery CDN is used only for jQuery lessons.
- The preview checks each lesson locally. It is a learning aid, not a production code security review.
