# Image Fix Notes

The KnowledgeOps screenshot now uses a valid HTML image block with straight quotes and a closing `>` on the `<img>` tag.

Correct image path:

`/assets/images/knowledgeops-demo.png`

Correct block:

```html
<a href="{{ '/assets/images/knowledgeops-demo.png' | relative_url }}" target="_blank" rel="noopener" class="screenshot-link">
  <img
    src="{{ '/assets/images/knowledgeops-demo.png' | relative_url }}"
    alt="KnowledgeOps Copilot desktop app screenshot"
    class="clickable-screenshot"
  >
</a>

<p class="image-caption">
  Click image to view full resolution.
</p>
```

After replacing your local site folder, push with:

```powershell
cd "$env:USERPROFILE\Desktop\spitnik11.github.io"
git add -A
git commit -m "Fix KnowledgeOps screenshot image path"
git pull origin main --rebase
git push
```
