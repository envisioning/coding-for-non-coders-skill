# Practical techniques come from people who build every day

The guide collects techniques from people who build with AI every day. They are sorted here by when the coach needs them. Pass one on when it fits the moment. A first session needs only a few.

## Some techniques help before the first prompt

- Build for yourself first. The person is the best judge of whether it works, and they will keep using it and improving it.
- Automate your own work first. A repetitive spreadsheet task, a weekly report or a reminder has the motivation built in.
- Start smaller than you think. Break work into the smallest chunks, smaller than feels necessary. Small requests give more accurate results than big multi-step prompts.
- Plan before coding. For anything bigger than one screen, use the AI to write a short plan first: what the app does, what data it keeps, the colors and the structure. Save the plan as a file and refer to it, so later changes stay consistent.
- Map it out first. Ask the AI to review the data and the logic and propose simplifications before it writes code.
- Know easy problems from hard ones. Screens, styling and simple lists of records are easy. Logins, moving data between formats and complicated app state are hard and need careful guidance.
- Know when AI is the wrong tool. Sometimes a no-code tool (Notion, Airtable, Zapier) or a developer is the better choice. For complex integrations, compliance or guaranteed reliability, vibe coding gets you a prototype and stops there.

## Some techniques help while building

- Details matter. A prompt with some depth (notes, examples, a clear summary of what you want) often works better than a terse one.
- Use more than text. Screenshots of a problem, of an error or of a design they like help the AI understand faster than a description.
- Paste the full error, every time. "It doesn't work" leaves the AI guessing. The complete error message usually leads straight to the fix.
- Tell the AI when something worked. It helps keep the style and the patterns the person likes.
- Read the responses. Ask the AI to summarize what it changed, so nothing slips in unnoticed.
- Let the AI explain the code. Ask what a file does, then ask follow-up questions. Each concept the person understands makes the next project easier. "What is an API?" "Why do I need environment variables?" "What does this error mean?"
- Share the documentation. When the app uses a specific service or library, paste its documentation into the conversation. Check that it matches the version the project uses.
- Use different models for different tasks. When one model struggles, another one may not.
- Blame the setup before the model. When the AI gets it wrong, it is usually a missing rule, a vague instruction or a chat full of noise. Fix what you gave it before switching tools.
- Keep a rules file (Claude Code). A file named `CLAUDE.md` or `AGENTS.md` holds the project's stack, conventions and hard rules. Start with ten lines. Each time the AI does something the person did not want, add a rule.

## AI makes the same mistakes again and again

- Changes nobody asked for. The AI may edit parts it was not asked to touch. Check the whole result after each change.
- Duplicate files. The AI can create a second file for the same job and edit the wrong one.
- Big deletions. To fix one problem, a model sometimes removes working code. Watch for features that disappear.
- Made-up details. The AI can mix tools, name things inconsistently or call services that do not exist.

## A few moves get you out when it breaks

- Fix one error at a time.
- Point to working code. Show the AI a part that works in a similar way.
- Add logging. Messages printed to the browser console show what the app is doing. The AI can place them.
- Rewind and retry. At a dead end, go back to the last working version, combine what you learned into one cleaner prompt, and try again.
- Know when to restart. A clean restart with lessons learned can be faster than untangling a mess.
- Step away. Fresh eyes catch what tunnel vision misses.

## A tidy project is easier for the AI (Claude Code)

- Work in separate files, and split a file once it grows past a few hundred lines.
- Avoid files with the same name in different folders. The AI confuses them.
- Use branches to try bold changes safely.
- Commit small changes one at a time, each in a working state.
- Keep development (trying things), build (checking that it compiles) and production (the live app) apart.
- Get it working first. Then get it right. Then get it fast. Ship the rough version, learn from it, and improve it.

## The same skills work beyond websites

The same skills work for data analysis scripts, Slack bots, browser extensions, automations and mobile apps. If the person can describe it, the AI can help build it.
