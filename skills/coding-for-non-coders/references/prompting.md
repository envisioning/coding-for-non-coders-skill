# A beginner can write a good prompt

This is the guide's first level, the Vibe Coder: prompt it, ship it. The goal of the level is to go from idea to working prototype in minutes. The steps are prompt, generate, iterate, preview and publish. Teach these techniques as the person needs them. Do not lecture all of them up front.

## The prompt says what you want

- Natural language. No special syntax is needed. The person says what they want in their own words, in any language. Say what you want and let the AI pick how: "Let users filter by date" works better than "Add a date picker component".
- "Build me a...". Starting with "Build me a..." or "I need a..." turns an idea into a first version. The AI picks the technology if the person does not. Example: "Build me a todo app that..." plus one constraint, such as "with dark mode".
- Ask for questions. Before the AI guesses anything, the person ends the prompt with "Ask me any questions you need before starting" or "What else do you need to know to build this properly?" This brings up missing details before any code exists. As the coach, you ask these questions yourself, a few at a time.
- Keep it simple. The simplest version that works beats an overbuilt one that might work. Start with the main path through the app, and add more only when it is needed. Useful lines: "Keep it simple, no extra features" and "Build the simplest version that does X. We'll add Y later."
- Markdown. Headings and lists make a longer prompt easier to read for people and for models. A useful shape: `## Goal`, `## Constraints`, `## Example output`.

## Generate gives a first draft

- Single prompt. One message in, a first draft out. No setup.
- Prototype. A small version that proves the idea works: one screen, one flow. It is the fastest way to see something real and get feedback.

## Iterate means asking again

- Refinement. The first output is rarely right. The person asks again with more detail ("make the button blue", "use my timezone") until it matches what they want. When there is an error, they paste it and ask "Fix this specific error". They do not need to explain the whole task again.
- Start over. If the code is messy or heading the wrong way, starting fresh is often faster than fixing. Useful lines: "This is too complex. Let's start over with a simpler approach." and "Forget that code. Build me a clean version that does X, Y, Z."

## Preview shows the app run

The person sees the app run and clicks through it. In Claude.ai that is the Artifact preview. In Claude Code it is a localhost address in the browser. See `surfaces.md`.

## Publish puts it in front of others

A share link from the tool, or an export of the code to put it somewhere else. See `publish.md`.

## One question helps with every prompt

The guide's advice for when a prompt does not work: stop looking for magic words. Ask what a new teammate would need to know to do this well. That is the goal, the constraints, and an example of the result. Help the person give you those three things.
