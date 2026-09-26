# Sudhansh Arora · Portfolio

Three role-specific portfolio sites for **Sudhansh Arora**, plus a landing page that lets a visitor pick the role they're hiring for.

| Path | Role | Design |
|---|---|---|
| `/` | All roles | Landing page with a link to each site |
| `/ai-qa/` | AI QA | **SudhanshOS**, a Windows-style desktop. The CV opens in Notepad, projects live in File Explorer, user stories in Sticky Notes. |
| `/ai-governance/` | AI Governance | **Model Card**. His experience written as an AI model card: overview, intended use, evaluation, builds, changelog, known limitations. |
| `/business-analyst/` | Business Analyst | **Requirements Board**. A movable whiteboard, from messy problem to signed-off delivery. |

Every site has light and dark mode, works on phones, and works with a keyboard.

## Folder structure

```
.
├── index.html                  landing page
├── ai-qa/index.html            SudhanshOS (AI QA)
├── ai-governance/index.html    Model Card (AI Governance)
├── business-analyst/index.html Requirements Board (Business Analyst)
├── assets/
│   ├── sudhansh-arora.jpg      profile photo
│   └── favicon.svg             browser tab icon
└── README.md
```

Plain HTML, CSS and JavaScript. No build step, no framework, no dependencies. Fonts load from Google Fonts.

## Links for applications

Send the link that matches the job:

- AI QA: `https://<your-domain>/ai-qa/`
- AI Governance: `https://<your-domain>/ai-governance/`
- Business Analyst: `https://<your-domain>/business-analyst/`

The AI QA desktop also opens a specific window from the link:

| Link ending | Opens |
|---|---|
| `/ai-qa/#cv` | CV in Notepad |
| `/ai-qa/#projects` | Projects (Portfolio Sites) |
| `/ai-qa/#stories` | User stories |
| `/ai-qa/#about` | About and achievements |
| `/ai-qa/#mail` | Email compose window |

## Run it locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Go live for free

**Option A: GitHub Pages**
1. Push this folder to a public repo, for example `Sudhansh3110/portfolio`.
2. In the repo, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then save.
4. The site goes live at `https://sudhansh3110.github.io/portfolio/` within a few minutes.

**Option B: Cloudflare Pages** (unlimited bandwidth)
1. Push this folder to GitHub.
2. In the Cloudflare dashboard, go to **Workers & Pages → Create → Pages → Connect to Git** and pick the repo.
3. Leave the build command empty and set the output directory to `/`.
4. Every push to `main` updates the live site.

Either option can use a custom domain later, such as `sudhansharora.com`.

## Adding a new Version 2.0 project

Each project needs a name, one-line description, user story, acceptance criteria (Given / When / Then) and what was built with. Add it in three places:

| Site | Where in the file |
|---|---|
| `ai-qa/index.html` | `SHIPPED` object and the folder list in `renderExplorer`. Add a sticky note under `<div class="stickies">`. |
| `ai-governance/index.html` | Copy the `<article class="build">` block inside `<section id="builds">`. Update the Evaluation “Build shipped” count. |
| `business-analyst/index.html` | Add a sticky inside the `f-delivered` frame. |

## Contact

- Email: arorasudhansh31@gmail.com
- LinkedIn: https://www.linkedin.com/in/sudhansh-arora/
- GitHub: https://github.com/Sudhansh3110

## Credits

Designed and built by Sudhansh Arora with Claude. Screenshots and link checks run with Playwright.
