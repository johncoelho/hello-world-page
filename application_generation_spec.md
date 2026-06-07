# Application Generation Spec

This repository follows this protocol whenever the user asks to create, generate, or build an application.

## Default stack

- Frontend: `HTML + CSS + vanilla JS`
- Backend: `Supabase`
- Database: `PostgreSQL` via Supabase
- Frontend SDK: `@supabase/supabase-js` loaded from `esm.sh`
- Hosting target: `GitHub Pages` or `Surge`

## Hard rules

- Do not use local Flask, FastAPI, Express, Node servers, or tunnels.
- Do not use SQLite as the main database.
- Prefer a static web app with a single `index.html` when possible.
- Use inline `<style>` and `<script>` for self-contained apps unless modular files are clearly needed.
- Use a dark tech-noir visual language with glassmorphism, subtle glow, and responsive layout.
- When persistence is needed, wire the UI to Supabase with the public anon key only.
- Never place secret server keys in the frontend.

## Visual direction

- Background: deep dark tones with animated particles or subtle atmosphere.
- Typography: modern sans-serif for UI, monospace accents for status/meta.
- Components: rounded cards, soft borders, frosted surfaces, clear hierarchy.
- Interaction: visible success and error states, hover elevation, loading feedback.

## Data pattern

- For lead/contact-style forms, use a table such as `leads` in Supabase.
- Prefer simple schemas that are easy to deploy and secure with RLS.
- Include setup instructions in `README.md` when persistence is involved.

## Expected output

- A complete app-ready project.
- `index.html` as the main entry point.
- Optional supporting files only when necessary.
- A project that can be deployed to static hosting without a custom backend.
- The local generator should use Codex CLI, save the files in `D:\sourcecode\<project>`, publish to GitHub Pages, and open the final public URL in the browser.
