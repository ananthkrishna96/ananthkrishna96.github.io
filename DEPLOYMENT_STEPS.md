# Deployment steps

You already created the correct repository:

```text
git@github.com:ananthkrishna96/ananthkrishna96.github.io.git
```

## Recommended local workflow

1. Clone the repository:

```bash
cd ~/Documents
git clone git@github.com:ananthkrishna96/ananthkrishna96.github.io.git
cd ananthkrishna96.github.io
```

2. Copy all files from the prepared website package into this cloned folder.

If the prepared folder is named `ananthkrishna96.github.io`, you can use:

```bash
rsync -av --delete /path/to/prepared/ananthkrishna96.github.io/ ./ --exclude .git
```

3. Check the changed files:

```bash
git status
```

4. Commit and push:

```bash
git add .
git commit -m "Create academic personal website"
git push origin master
```

If your branch is `main`, use:

```bash
git push origin main
```

5. Wait a few minutes and open:

```text
https://ananthkrishna96.github.io/
```

## GitHub Pages settings

Go to:

```text
Repository -> Settings -> Pages
```

Use:

```text
Source: Deploy from a branch
Branch: master or main
Folder: /root
```

The correct branch is the branch visible on your repository's Code page.

## First checks after publishing

- Homepage loads correctly.
- Profile photo appears in the left sidebar.
- CV download works.
- Research page opens.
- Projects page lists project cards.
- Publications page shows the master's thesis entry.
- Talks page shows SIMAI 2025, SAMM 2025, and Dobbiaco 2023.
- Contact links open correctly.
- No full street address or phone number appears on the website.
