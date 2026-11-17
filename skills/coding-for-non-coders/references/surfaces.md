# Each tool changes where the code lives

The method is the same everywhere: describe, build, look, change, save, share. What changes is where the code lives, how the person sees it run, and how they save versions.

## Claude.ai and the Claude desktop app

- Where it runs: you build in an Artifact. The preview shows in the chat, and the person clicks through it right there. Nothing to install.
- What to build: one self-contained page (HTML, CSS and JavaScript in one file, or a single React component). Keep data in the page or in the browser, with sample data to start.
- Saving versions: earlier versions of the Artifact stay in the conversation. When a version works, say so, so the person knows which one to go back to.
- When the chat gets long and confused: ask the person to start a new chat, and give them a short summary to paste in: what the app does, what works, what is broken, and the latest code if they need it.
- Sharing: the Artifact can be published and shared as a link from the Artifact view. See `publish.md`.
- Limits: no terminal and no hosting of a backend. Logins, a shared database and secret keys are out of reach here. That is fine for a first prototype.

## Cowork

- Where it runs: you write files into a folder the person picked. They open the HTML file in their browser by double-clicking it, or by dragging it into a browser window.
- What to build: one HTML file with everything in it. Tell the person the exact file name each time you change it, and ask them to reload the browser page.
- Saving versions: before a big change, copy the working file with a version in the name, for example `habits-v2.html`.
- Sharing: send the file, or follow the website walkthrough in `publish.md`.
- Limits: same as Claude.ai. No secrets in the files.

## Claude Code

- Where it runs: you have a terminal on the person's computer. Make one new folder for the project and work only inside it.
- What to build: start with one HTML file if the idea allows it. If the idea needs a framework, pick a common one and keep it small. Run it with the project's dev command and give the person the localhost address to open, for example http://localhost:3000. Localhost means the app runs on their computer. Nothing is live until they deploy.
- Before each command, say in one plain sentence what it does. Do not install large tools without asking. If a tool the project needs is missing, tell the person what it is and ask before installing it.
- Saving versions: initialize Git in the project folder. Commit when something works, with a short message that says what changed. Use a branch for a risky change.
- Secrets: they go in `.env`, which the person fills in with a text editor. Add `.env` to `.gitignore` before the first commit. Never print a secret, and never ask for its value in the chat.
- A rules file: when the project grows, create `CLAUDE.md` in the folder with the stack, the conventions and the rules the person cares about. Each time you do something they did not want, add a rule. See `techniques.md`.
- Sharing: push to GitHub and connect the repository to a one-click host. See `publish.md`.

## Other chat tools work the same way

The guide's first ten minutes also work in ChatGPT (Canvas) and Google AI Studio. All three have free tiers. If the person uses another tool, the same coaching steps apply.
