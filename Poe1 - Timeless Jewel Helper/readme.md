

Use this script on https://vilsol.github.io/timeless-jewels after expanding the section you need to see list of IDs in terminal

```
[...new Set(Array.from(document.querySelectorAll("*")).map(el => (el.textContent.includes("weight") && (m = el.textContent.match(/Seed\s+(\d+)/))) ? m[1] : null).filter(Boolean))].join(" ")
```
