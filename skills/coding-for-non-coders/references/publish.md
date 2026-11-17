# Sharing is optional and publishing takes a few clicks

A prototype that runs on the person's own screen is a complete result. Publishing is optional. Before anything goes public, check together that it contains no secrets (keys, passwords, tokens) and no real personal data.

## A share link is the quickest option

Many AI tools give a link to a prototype. Sharing it with friends or colleagues is the fastest way to get feedback before anyone spends time on a real website.

- Claude.ai and the desktop app: the Artifact can be published and shared as a link from the Artifact view.
- Export: the person can also copy or download the code and keep it. That is how a project moves out of the chat tool and becomes theirs.

## The guide's walkthrough puts a website live with v0, GitHub and Vercel

The guide's simplest path is: build in v0, save to GitHub, deploy with Vercel. If you can click buttons, you can ship a website.

- GitHub is where the project code lives, in a "repository".
- Vercel is one-click hosting that publishes the site at a live address.
- v0 is a project hub to build, publish and manage settings.

The steps from the guide:

1. Create accounts. Sign up at vercel.com first. Then go to v0.app and log in with "Continue with Vercel". Then create a github.com account, so v0 can create a repository.
2. Build something in v0. The guide's exercise prompt: "Build a website for a bakery that fits the vibe of (city, country)." Select the model "Auto".
3. Publish. Top right in v0, click "Publish".
4. Create the repository. Click "Create repository", connect GitHub in the popup, then click "Create repository" again.
5. Publish to production. Click "Publish" again, then "Publish to production". The site is live.

To change the random address Vercel gives the site: go to v0.app/projects, click the project name, open the three-dot menu, click "Settings", then "Domain", type the new name and click "Save". With their own domain, Vercel may ask them to add a DNS record. That is normal.

The person creates every account and enters every password themselves. You guide them through the screens.

## Claude Code can put the same project live

When the project already lives in a folder on the person's computer, the same two services do the job:

1. The person creates a GitHub account and a Vercel account, if they have none.
2. You commit the working version, create a repository on GitHub and push the code. Explain each command in one sentence before you run it. If the GitHub command-line tool is not signed in, the person signs in themselves.
3. The person opens Vercel, chooses to add a new project, and imports the repository. Vercel builds it and gives a live address.
4. If the app uses secret keys, the person adds them in the Vercel project's environment variables settings. They never go into the code or the chat.

If the deploy fails, ask for the entire error message from the Vercel build log. Netlify works the same way and is a good alternative.
