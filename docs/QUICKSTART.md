# Comic Explainer: your first visual training story

By Mark Kentwell · Adapted from Ian Xiaohei Illustrations by Ian (@ianneo_ai) · MIT

## What is a skill?

A skill is a saved set of instructions for an AI agent. It tells the agent how you want a particular job done: what to look for, what to make and how to check it. Comic Explainer teaches the agent to turn a dense explanation into a sequence of simple, memorable pictures.

It is not an app or a new model. Your agent still needs access to an image-generation tool to make pictures. Without one, it can write the storyboard and prompts for you to use with a renderer.

## Get the pack

Go to [Comic Explainer](https://comic-explainer-by-mk.netlify.app/). Download the ZIP and quick-start PDF. The ZIP contains one installable skill folder, its supporting references, the licence and this guide.

For Codex, copy the complete `comic-explainer` folder into `~/.codex/skills`, or the `skills` folder in your custom CODEX_HOME. If a version is already there, preserve it before replacing anything. Use a new agent session, then ask for `$comic-explainer`. The repo README has terminal instructions if you prefer them.

For another agent, use its own skill installation method. Do not assume every chat app can install a SKILL.md file. You can also supply the skill and references as instructions in a chat; image generation still depends on that app's tools.

## Bring one real idea

You do not need a polished script. Start with a voice-note transcript, a rough explanation, an existing training document or a how-to. Include:

- Who it is for.
- What they are finding difficult.
- The one idea you want them to remember.
- What they should do afterwards.
- How long you have to explain it.

Use non-confidential material for your first public example. Decide what is allowed to be shared before asking for a public website.

## Copy this prompt

```text
Use $comic-explainer.
My audience is [who].
They currently struggle with [specific problem].
The idea I want them to remember is [one sentence].
Afterwards they should [one action].
I have [10 / 15 / 20] minutes to deliver it.

Turn my explanation into [six / nine] comic scenes.
Label everything in English. Use white backgrounds, black hand-drawn
linework and a recurring character doing the explanatory action.
Generate each picture separately using the image tools available here.
Add a short headline, one takeaway and talking points to each scene.
Keep caveats and long explanations in the notes.

Here is my explanation:
[Paste it here.]
```

## Three ways to use it

**Plan first.** Add “Storyboard and prompts only. Do not generate images yet.” Use this when the idea is still being shaped.

**Make the pictures.** Ask for individual rendered scenes. The agent should inspect each one and fix labels or visual logic before finishing.

**Make a presentation.** Add “Build an interactive website with arrow-key navigation, expandable detail, presenter notes and a clean recording view. Prepare locally first.” Name the host and explicitly request publication when ready. A request for a comic does not automatically publish it.

## Give feedback that fixes the right thing

Useful feedback is specific:

- “Scene 2 mixes two ideas. Keep only the missed decision point.”
- “The character should actually open the gate, not stand beside it.”
- “The tally says twenty but there are fifteen marks. Correct just the marks.”
- “Both water surfaces need to align for this metaphor to make sense.”
- “Move that paragraph into a pop-out; leave three labels in the image.”

Ask for one targeted edit. If the spatial structure is still confused after an edit or two, ask to regenerate that scene with the relationship described clearly.

## Deliver it

Use the images as the memory anchors. Talk through the example rather than reading every label. Pause at the biggest reframe. Practise one useful sentence. End with a small next action.

For a recorded walkthrough, use the clean recording view. Download speaker notes to a second screen if you need prompts outside the video. Notes on a public website are still publicly accessible.

See [Mark's working nine-scene example](https://presence-four-ways-sales.netlify.app/#1). Arrow keys move through it; N opens notes; F switches to Loom mode. The illustrative depth and campaign numbers are teaching examples, not market rules.

## Remember the two names

**Comment EXPLAINER** is the keyword for the video offer. **Comic Explainer** is the skill name. Inside a compatible installed agent, invoke **`$comic-explainer`**.

## Credit and licence

The original illustration skill and Xiaohei visual language are Ian's. Mark adapted the workflow for training, how-to comics and interactive delivery. Keep the bundled licence and notices when sharing or modifying the package. You can use it commercially under MIT. Image-model terms and rights in material you upload remain separate.

Read [MIT explained](LICENCE-EXPLAINED.md), [the licence](../LICENSE) and [the upstream project](https://github.com/helloianneo/ian-xiaohei-illustrations).
