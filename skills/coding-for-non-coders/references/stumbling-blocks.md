# Everyone hits the same stumbling blocks

Everyone hits these. Tell the person that they are normal. That makes them easier to push through. For each one: what the person says, what is going on, and what you do.

## "It worked, then I changed one thing and everything broke"

AI sometimes makes changes nobody asked for, and they spread. The fix is saved versions.

What you do: go back to the last version that worked. Then make the change again, smaller. From now on, save a version each time something works (Git commits in Claude Code, a noted Artifact version in Claude.ai, a file copy in Cowork).

## "The AI keeps going in circles"

When a fix for one thing breaks another, again and again, the conversation has gone stale. The model is working from piled-up confusion.

What you do: say so. Write a short summary of what the app does, what works and what is broken. Suggest a new chat with that summary pasted in. Fresh context usually breaks the loop.

## "I don't understand the code it wrote"

The person does not need to understand every line. They should understand what each file does and how the pieces connect.

What you do: explain it as if they have never coded before. Do this regularly, without being asked, after each bigger change.

## "My app looks ugly"

AI defaults work but look generic. Design takes rounds of changes, like code. The person has to be specific about the look they want.

What you do: ask for a screenshot of a design they like, and build toward it. Ask about colors, spacing and the feel they want, one at a time.

## "I can't get it to deploy"

Getting from "works on my computer" to "works on the internet" trips up everyone. Build errors, environment variables and hosting settings are the usual blockers.

What you do: start with a one-click platform such as Vercel or Netlify. Ask the person to paste the entire error message, never a summary. See `publish.md`.

## "It looks right but does the wrong thing"

The mistakes AI makes have changed. They used to be obvious crashes. Now the code often looks clean, runs, and is quietly wrong: a total that is off, a case it missed, the wrong item updated. It can pass a quick test.

What you do: check what the app does, beyond whether it runs. Ask the person to try real and odd inputs and compare the result with what they expect. "It didn't error" and "it's correct" are two different claims.

## "I'm spending more time debugging than building"

This is the job. Experienced developers spend 30 to 50 percent of their time debugging. The share goes down with experience and never reaches zero.

What you do: tell them it is normal. Ask for the full error each time. In a browser app, show them the developer tools (F12) and where error messages appear there.
