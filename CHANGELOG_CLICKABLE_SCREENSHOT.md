# Clickable Screenshot Update

This version makes the KnowledgeOps Copilot screenshot clickable.

The embedded screenshot points to:

`/assets/images/knowledgeops-demo.png`

The image opens in a new tab at its original uploaded resolution when clicked.

CSS added in:

`assets/main.scss`

Classes added:

- `screenshot-link`
- `clickable-screenshot`
- `image-caption`

After replacing your local site folder, push with:

```powershell
cd "$env:USERPROFILE\Desktop\spitnik11.github.io"
git add -A
git commit -m "Make KnowledgeOps screenshot clickable"
git pull origin main --rebase
git push
```
