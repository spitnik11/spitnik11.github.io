# Screenshot Display Update

This version reverts the KnowledgeOps screenshot to a normal embedded image instead of a clickable full-resolution link.

The screenshot path is:

`/assets/images/knowledgeops-demo.png`

The KnowledgeOps post uses:

```html
<figure class="screenshot-figure">
  <img
    src="{{ '/assets/images/knowledgeops-demo.png' | relative_url }}"
    alt="KnowledgeOps Copilot desktop app screenshot"
    class="project-screenshot"
  >
  <figcaption>
    KnowledgeOps Copilot running locally with source-backed answers and document search results.
  </figcaption>
</figure>
```

Styling was added to `assets/main.scss` to make the image larger, clearer, and easier to see.

After replacing your local site folder, push with:

```powershell
cd "$env:USERPROFILE\Desktop\spitnik11.github.io"
git add -A
git commit -m "Revert screenshot to normal embedded display"
git pull origin main --rebase
git push
```
