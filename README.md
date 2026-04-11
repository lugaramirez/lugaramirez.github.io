# Speaking about AI

A slide deck about how to start with AI at work — covering agents, hallucinations, and what AI actually is under the hood. Built for developers but accessible to non-developers.

**Three sections:**
1. Getting agents to work for you (Claude Code, Claude Desktop, practical setup)
2. Avoiding hallucinations in production (context limits, prompt poisoning, guardrails)
3. AI is not intelligent — it's a statistical model (and that's okay)

---

## Presenting

### Slide deck

Open the deck in your browser:

<a href="https://lugaramirez.github.io/" target="_blank" rel="noopener">lugaramirez.github.io ↗</a>

| Key | Action |
|-----|--------|
| `→` / `↓` / `Space` | Next slide |
| `←` / `↑` | Previous slide |

---

### Presenter view (two-tab mode)

The deck supports a synchronized presenter view. Both tabs stay in sync — navigating in either one updates the other.

**Step 1 — Open the slide deck** (your main display / projector tab):

<a href="https://lugaramirez.github.io/" target="_blank" rel="noopener">Open slide deck ↗</a>

**Step 2 — Open the presenter notes** (your laptop tab):

<a href="https://lugaramirez.github.io/?view=notes" target="_blank" rel="noopener">Open presenter notes ↗</a>

The notes tab shows:
- Current slide number and section
- Speaker note for the active slide in large readable text
- "Up next" preview with the title of the following slide

If you open the notes tab while the deck is already mid-presentation, it will immediately sync to the current slide.

---

## Editing

Everything lives in a single `index.html` file. To add a slide:

1. Copy any `<div class="slide">` block inside `#viewport`
2. Set `data-section="Your Section Name"` on the div
3. Edit the content — slides render in DOM order

To add speaker notes to a slide, include:

```html
<aside class="speaker-note">Your note here.</aside>
```

Notes are hidden from the audience view and only appear in the presenter tab or when pressing `N`.
