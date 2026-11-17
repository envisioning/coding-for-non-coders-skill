# Coding for Non-Coders skill

This skill turns your AI agent into a coach for building software when you do not code. You describe an idea, the agent builds a first version, you look at it and ask for changes, and you end with a working prototype that you built yourself.

The coach follows Envisioning's open guide, [Coding for Non-Coders](https://www.envisioning.com/coding-for-non-coders). It helps you pick a small idea, write your first prompt, see the app run, change it one request at a time, save the versions that work, and share the result if you want to. It is honest about the hard parts, and it tells you what to do when things break.

The skill is free and public. It works in Claude.ai, the Claude desktop app, Cowork and Claude Code.

## You start by saying what you want to build

- "I want to build an app but I can't code."
- "Help me make a prototype of a habit tracker."
- "Teach me vibe coding."
- "Can you help me turn my spreadsheet into a small app?"

## Each tool works a little differently

- In Claude.ai and the Claude desktop app, the coach builds in an Artifact, so you see the app run right in the chat. You install nothing.
- In Cowork, the coach writes the app as a file in a folder you pick, and you open it in your browser.
- In Claude Code, the coach also uses the terminal: it creates a project folder, runs the app on your computer, saves versions with Git and can help you publish to the web.

## Your passwords and keys stay out of the chat

The coach never asks you to paste a password, an API key or a token into the chat. In Claude.ai and Cowork it builds prototypes that need no secrets. In Claude Code, secrets go in a `.env` file that you fill in yourself and that never goes to GitHub. On a hosting service, they go in the service's environment variables settings.

## The repository holds the skill and two manifests

- `skills/coding-for-non-coders/SKILL.md`: the coaching steps the agent follows.
- `skills/coding-for-non-coders/references/`: the guide's prompts and project ideas, prompting techniques, stumbling blocks, practical techniques, publishing steps, expectations, and the differences between tools.
- `.claude-plugin/`: the Claude Code plugin and marketplace manifests.

The skill needs no MCP server and no account with us.

## You install it in one of three ways

### Claude Code

In a Claude Code session, run:

```
/plugin marketplace add envisioning/coding-for-non-coders-skill
/plugin install envisioning-coding-for-non-coders@envisioning-cfnc
```

Then say what you want to build, and Claude uses the skill. You can also call it directly with `/envisioning-coding-for-non-coders:coding-for-non-coders`.

### Claude.ai, the Claude desktop app and Cowork

If you find the plugin in the Claude plugin directory, install it from there. Otherwise:

1. Download this repository and zip the `skills/coding-for-non-coders` folder.
2. In Claude, open Settings, then Capabilities, and upload the zip under Skills.

### Other agents

`skills/coding-for-non-coders/SKILL.md` follows the Agent Skills format, so it works in any agent that supports that format. Copy the `skills/coding-for-non-coders` folder to wherever your agent loads skills from.

## Teams can learn this together

We also run this guide in person as Build Sessions: a half-day session where up to 10 people each build a prototype of their own, with one facilitator. See https://www.envisioning.com/services/build-sessions.

## The text is CC BY 4.0 and the code is MIT

The skill text is CC BY 4.0. The code and configuration are MIT. See `NOTICE.md` and `LICENSE`.

Made by Envisioning, https://www.envisioning.com
