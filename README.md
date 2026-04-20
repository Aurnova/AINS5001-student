# AINS5001-student — Aurnova

**Live site:** https://aurnova.github.io/AINS5001-student/

**Audience:** **Students** — single public entry for **GitHub Classroom + Codespaces + exercises**. This repo does **not** ship instructor solutions, IMS CC exports, or the full narrative bundle; those stay on the **[instructor hub](https://aurnova.github.io/AINS5001/)** and Castalia/private channels.

## Build (Pages)

Same static shell as **AINS5001**; `variant.json` sets `audience: "student"`.

```bash
npm install
npm run build
```

Optional: add your **Classroom assignment** URL under `navItemLinks.Assignments` in `variant.json` so the sidebar **Assignments** item becomes a link.

## Create the GitHub repo

This folder is ready to `git init` and push to **`Aurnova/AINS5001-student`** so Pages serves at `https://aurnova.github.io/AINS5001-student/`.

```bash
cd AINS5001-student
git init -b main
git add .
git commit -m "Add student-facing AINS5001 Pages site"
gh repo create Aurnova/AINS5001-student --public --source=. --remote=origin --push
```

Enable **GitHub Actions → Pages → GitHub Actions** as the source for that repository.

## License

Content policy matches the parent AIMA / Castalia programs licensing workflow.
