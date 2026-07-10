# Setup

This profile works immediately after pushing.

## 1. Repository name

This must live in a repository named exactly like your username:
`Dey70/Dey70`. GitHub only renders a
profile README from that special repo.

## 2. Enable the snake workflow (one-time)

The contribution snake needs Actions to run once before it appears:

1. Push this repo to `Dey70/Dey70`.
2. Go to **Settings → Actions → General → Workflow permissions** and select
   **Read and write permissions**.
3. Go to the **Actions** tab, open **Generate Snake Animation**, and click
   **Run workflow** once manually. After that it runs nightly on the
   schedule in `.github/workflows/snake.yml`.
4. This creates an `output` branch holding `dist/snake.svg`,
   `dist/snake-dark.svg`, and `dist/snake-light.svg` — already referenced
   in the README, so no further edits are needed.

## 3. Stats cards

The GitHub stats, streak stats, top languages, activity graph, and trophy
images call public hosted APIs (`github-readme-stats`, `github-readme-streak-stats`,
`github-readme-activity-graph`, `github-profile-trophy`). They work with
just your username in the URL — no deploy of your own instance required.
If you ever hit their rate limits, each project has instructions for
deploying a free personal instance on Vercel.

## 4. Sections intentionally left out

Experience, Achievements, Certifications, and Coding Profile (LeetCode /
GeeksforGeeks / HackerRank / CodeChef) sections were left out of this
README rather than filled with placeholder or invented content. Add them
yourself when you have real details to put in — copy the collapsible
table pattern used in the Featured Projects section for consistency.

## Optional: unused assets

`assets/banner.svg` and `assets/footer.svg` are no longer referenced —
the header and footer now use hosted Capsule Render banners instead.
Keep or delete them as you like. `assets/icons/` is still reserved if you
want custom tech-stack icons later.
