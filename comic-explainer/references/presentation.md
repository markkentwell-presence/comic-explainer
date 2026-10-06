# A comic people can present and revisit

Prefer a lightweight static website when the user wants a link they can update and share. Use another format when requested. Build only what the delivery needs.

## Viewer experience

- One large illustration, short headline and one takeaway per scene.
- Previous/next controls, a scene counter and direct links such as `#3`.
- Arrow keys, an overview and first/last boundaries that behave predictably.
- Extra-detail bubbles that work on hover, keyboard focus and tap. Give each an explicit close action. Ensure closing and restoring focus do not immediately reopen it.
- A phone layout without horizontal overflow. Keep the take-home guide accessible on a phone.
- Useful alternative text and visible keyboard focus. Avoid depending on colour alone.

## Presenter experience

Offer a notes view, suggested pace per scene and optional start/pause/reset timer. A recording mode hides notes and detail controls while preserving simple navigation. Explain that notes on a public website are public; downloading them to a second screen is a way to keep them out of the video, not access protection.

Keep timing tied to elapsed time rather than assuming every timer tick runs exactly on schedule. Keep long qualifications in notes so the core visual remains readable.

## Publish and update

Use the user's requested platform and existing authorised account. Do not change another site, repo visibility, account protection or paid plan to make deployment easier. If a public link is requested, make only the agreed content public. A general request for training does not authorise publication.

Keep editable scene content separate from navigation and styling. Use an explicit publish allow-list. Raw transcripts, personal context, private skill files, logs and credentials do not belong in a public publish directory. A noindex tag requests search exclusion; it is not a password.

Record the destination, release ID and file manifest. Preserve a prior release or archive so a later content change can be reversed through a fresh deployment of saved content. If a platform transforms HTML, distinguish its normal processing from a broken file; host configuration files may not be served publicly.

Verify the live URL and asset loading, not just a successful upload command. Do not claim continuous Git deployment unless it is actually configured.
