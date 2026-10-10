# AGENTS.md

Guidance for agents and humans working in `focalstudio/media`. This repo is **public**: anything pushed here is
downloadable by anyone, and git history keeps it forever.

## Rules
- Finals only: finished clips and images for posts. No drafts, sources, keys, screenshots of private data or unreleased work.
- Layout is `<app>/<clean-name>` (lowercase, `a-z0-9.-`), e.g. `wildfocus/wildfocus-meditate.mp4`, with a `.png` thumbnail beside each video.
- Never delete or rename a published file: marketing queue posts reference it by `media:` path, and Instagram and Threads fetch it late.
- Don't upload by hand. Use `node scripts/push-media.mjs <file> [app]` from `focalstudio/marketing`; it names the file, pushes it and prints the `media:` line.
- Branch off `main`, open a PR for anything beyond a media upload (docs, license). Never force-push.

## Layout
- `<app>/`: one folder per app.
- `README.md`: what the repo is. `LICENSE`: all rights reserved; the media is Focal Studio's.

## CHANGELOG
Media uploads are tracked by git history. Note only structural changes (new app folder, naming rule) in [CHANGELOG.md](CHANGELOG.md).
