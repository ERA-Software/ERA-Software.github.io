# Contributor guidelines

This page explains how members of the ERA group should publish and maintain repositories within the ERA-Software organization.

The goal is simple:

> Make research code reproducible, structured, and easy to reuse.

---

## What belongs on ERA-Software?

According to the GitHub workshop slides :contentReference[oaicite:1]{index=1}, repositories should typically contain:

- Supporting code for lectures
- Supporting software associated with the chair (e.g. ERADist → eraUQ)
- Code / algorithms associated with papers
- Reusable research tools

---

## What should NOT be uploaded?

GitHub is optimized for tracking **text files** :contentReference[oaicite:2]{index=2}.

Do **not** upload:

- Word documents
- PDFs
- Large datasets
- Notebook outputs
- Cache folders (e.g. `__pycache__`)
- Secrets, passwords, API keys
- Large binary files

Keep repositories clean and lightweight.

---

## How to publish a new repository

### 1. Prepare your local project

Your repository should contain:

- `.gitignore`
- `LICENSE`
- `README.md`

Use the ERA paper template as reference if needed :contentReference[oaicite:3]{index=3}.

---

### 2. Create a repository

You can:

- Create it under your personal account **or**
- Create it directly under `ERA-Software`

Repositories should normally be:

- **Private during development**
- Made public once stable and documented

---

### 3. Push your code

Basic workflow:

```bash
git init
git add .
git commit -m "Initial commit"
git push
```

Or use GitHub Desktop if preferred.

---

### 4. Fork if necessary

If you created the repository in your personal account:

- Fork it into `ERA-Software`

If it was created in ERA-Software:

- Keep development via branches or forks.

---

## Minimal repository standards

Every ERA repository should include:

### README.md

Must contain:

- Short description
- Installation instructions
- Minimal usage example
- Citation information (if linked to a paper)

### License

Choose an appropriate open-source license.

### Clean structure

Organize clearly:

```bash
project/
│
├── src/
├── tests/
├── README.md
├── LICENSE
└── .gitignore
```

---

## Collaboration rules

- Use branches for new features
- Use pull requests for merging
- Keep commit messages meaningful
- Do not push directly to main for major changes

---

## Final goal

We use GitHub to:

- Track intermediate code states
- Collaborate
- Share reproducible research