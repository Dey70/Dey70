# Setup

This profile works immediately after pushing, once you do two things:

## 1. Repository name

This must live in a repository named exactly like your username:
`Dey70/Dey70`. GitHub only renders a
profile README from that special repo.

## 2. Replace placeholders

Find & replace across `README.md` (and the `.github/workflows/snake.yml`
username line if you don't want to rely on `github.repository_owner`):

| Placeholder                                                                   | Replace with                     |
| ----------------------------------------------------------------------------- | -------------------------------- |
| `Dey70`                                                                       | your GitHub username             |
| `https://www.linkedin.com/in/rajdeep-dey-188784289/`                          | your LinkedIn handle             |
| `https://x.com/Observer_x70`                                                  | your X / Twitter handle          |
| `rajdeep.x70@gmail.com`                                                       | your email address               |
| `YOUR_PORTFOLIO_URL`                                                          | your portfolio URL               |
| `https://github.com/Dey70/observer-os-web.git`                                | actual repo name for Observer OS |
| `https://github.com/Dey70/WebNew-AI-Powered-Website-Translation-Platform.git` | actual repo name for WebNew      |
| `https://github.com/Dey70/WB-voice-translator.git`                            | actual repo name for KothaSetu   |
| `https://github.com/Dey70/EduGuardian-AI-Voice.git`                           | actual repo name for EduGuardian |

If a project repo is private or doesn't exist yet, either remove that
project's card or point the "Repository" button at `#` until it's ready.

## 3. Enable the snake workflow (one-time)

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

## 4. Stats cards

The GitHub stats, streak stats, top languages, activity graph, and trophy
images call public hosted APIs (`github-readme-stats`, `github-readme-streak-stats`,
`github-readme-activity-graph`, `github-profile-trophy`). They work with
just your username in the URL — no deploy of your own instance required.
If you ever hit their rate limits, each project has instructions for
deploying a free personal instance on Vercel.

## Optional: project images

`assets/icons/` is reserved if you want to drop in custom tech-stack icons
later. The project cards currently use shields.io badges instead of a
placeholder image so they render correctly with zero extra setup — swap in
real screenshots under `assets/` and update the `<td>` blocks in
`README.md` if you'd like actual preview images.
