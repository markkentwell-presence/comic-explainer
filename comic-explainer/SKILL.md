---
name: comic-explainer
description: Turn training concepts, voice notes, transcripts and how-to instructions into memorable hand-drawn comic explainers, with scene-by-scene illustrations, talking points and optional interactive presentation websites. Use for comic training, visual how-to guides, or “Comic Explainer”; ordinary illustration and software diagrams do not need this workflow.
license: MIT
---

# Comic Explainer

Turn a talk into a story people can see, remember and use. Adapted by Mark Kentwell from [Ian Xiaohei Illustrations](https://github.com/helloianneo/ian-xiaohei-illustrations) by Ian (@ianneo_ai), MIT. Keep the credit in redistributed skill packages; see [NOTICE.md](NOTICE.md).

Invocation: `$comic-explainer`, “Use Comic Explainer”, or `/comic-explainer` where the host supports slash skills. “Comment EXPLAINER” is a social distribution CTA, not an installed-agent command.

## Choose the deliverable

- **Plan only:** storyboard and image prompts; do not render if the user asks only for planning.
- **Make the comic:** generate each scene separately, check it, and save the final assets. Do not stop after a storyboard when the user asked for images.
- **Presentation or how-to website:** add a readable interactive deck with notes and expandable detail when requested. Publishing needs an explicit destination and authorisation; a skill invocation alone does not authorise cloud uploads or messages.

Use available image tools. In Codex, prefer the built-in image-generation tool when available. In other hosts, use an available image connector or the user's chosen renderer. Do not silently switch providers, incur unrequested paid services, install tools or retrieve credentials. If generation is unavailable, deliver the storyboard and prompts, state that images are not generated, and explain the smallest remaining requirement.

## 1. Find the idea and the action

Read the supplied material. Identify the audience, the behaviour to change, one core idea and a memorable physical metaphor. Use the audience's language. English labels and Australian spelling are defaults; honour the user's chosen language.

Distinguish facts from examples, coaching targets and metaphors. A three-level drawing is not automatically a three-step rule or a numerical claim. Check external facts when the story relies on them, and put qualifications in notes rather than crowding the picture.

Infer reversible presentation choices from the brief; ask only for information that materially blocks the work. Summarise the story direction briefly and proceed within the requested scope.

## 2. Build a sequence, not a pile of pictures

For a talk, usually 6–9 scenes; use fewer for a short how-to. Choose the count from the concept and delivery time. Do not force a fixed number.

Give each scene:

- One idea the viewer should remember.
- One visible action that explains it.
- A short headline and 3–6 short image labels; eight is the ceiling.
- A one-sentence takeaway.
- Presenter talking points, a suggested time and an optional question or practice move.
- Extra explanation only where it helps, for notes or pop-outs.

Build a recognisable progression: familiar problem → surprising reframe → physical metaphor → practical options → next action. A how-to may instead use a clear start, decision points and finish. Reuse the character and visual setting, not the same composition in every scene.

Read [references/story-design.md](references/story-design.md) when structuring a multi-scene talk or behaviour change.

## 3. Make the illustrations

Read [references/visual-language.md](references/visual-language.md) before prompting. Default: individual 16:9 images, pure white background, lightly irregular black linework, ample white space, and restrained handwritten labels. Orange shows movement; blue shows state; red flags a problem. Main text and objects are black.

Ian's recurring Xiaohei character is a small irregular solid-black creature with white dot eyes, thin arms/legs and a blank serious expression. It must do the action that explains the idea. Use a different character if requested; do not imply Ian created the adaptation or endorses it.

Keep the pictures mature, simple and a little unexpected. Invent a fresh, low-tech physical metaphor from the current concept. Avoid commercial infographic grids, dense course slides and copied example compositions.

Generate one scene per call, not a contact sheet. If independent calls can safely run together, keep each result mapped to its own scene. For generation results, record output paths and small metadata; never print base64 image payloads. Preserve originals. Save the selected outputs as `assets/<project-slug>-illustrations/01-topic.png`, etc., inside the user's designated output area.

Keep exact labels in the prompt and explicitly say “Label everything in English” or the chosen language. Never use capitalised stage directions that could become image text. Put full explanations in the presentation layer, not inside the generated image.

## 4. Inspect, fix and verify

View every generated scene. Check meaning first: is the character doing the right thing, are counts accurate, do depths/thresholds/paths agree with the metaphor, and is the outcome visible? Then check labels, style, whitespace and consistency.

For a local edit target, inspect the image before asking the image tool to edit it. Correct one precise defect and preserve the rest. After one or two ineffective edits, regenerate the scene with the geometry or action stated more clearly. Compare candidates and retain the best one; a later result is not automatically better.

Read [references/quality-check.md](references/quality-check.md) for the final review.

## 5. Deliver something usable

If a site was requested, read [references/presentation.md](references/presentation.md). Keep the large illustration and short takeaway on screen. Make extra detail available on hover, keyboard focus and tap. Provide keyboard navigation, direct scene links, a phone layout and presenter notes. A clean recording view should hide the notes and extra controls.

Talking points must fit the requested time; the suggested allocations should sum to that duration. Treat them as pacing guidance, not a claim of a human rehearsal. Finish with an action small enough to practise now, an owner and a review point where useful.

Verify links, scene order, image loading, navigation, pop-outs and any deployment before declaring completion. Keep an editable source, prompt set and selected assets. If publishing, upload only the agreed training deliverables; exclude raw transcripts, private contextual skills, credentials and incidental personal material. Preserve prior releases and record how to reverse a later content change by redeploying saved content.

Report the finished link or files, scene count, presenter controls and any concrete limitation. Do not claim an image, PDF or deployed site exists unless it does.
