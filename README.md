# Mercantile Gear Tracker

A single-file web app for tracking gear across video production jobs. Built with plain HTML, CSS, and JavaScript — no frameworks, no backend, no accounts. Runs in any browser and saves state locally.

**Features:**
- Job tabs with pack list, packed/returned tracking
- Pickup and return date pickers per job
- One-tap Google Calendar event publishing
- Rental days multiplier — daily rates × days = total
- Custom pricing overrides per job
- Custom gear items (per job or permanent)
- Archive completed jobs to a separate tab
- Works on mobile

---

## Make Your Own Version with Claude

Copy and paste the prompt below into [Claude](https://claude.ai). It will build you a customized version from scratch based on your own gear list.

---

### The Prompt

```
I want to build a gear tracking web app for my video production work — a single HTML file I can host on GitHub Pages and use on my phone.

Here's my gear list:

[PASTE YOUR GEAR LIST HERE — item names and daily rental rates if you have them. Categories help too, e.g. Camera, Lenses, Audio, Lighting, Grip, etc.]

The app should:
- Let me create jobs (name, date, client, number of rental days, pickup date, return date)
- Check off gear for each job from my master list
- Show a pack list at the top with packed and returned checkboxes
- Highlight selected gear in yellow, packed in green, returned in blue
- Show a running total: daily rates × number of rental days
- Let me override the price on any item per job by clicking the price
- Let me add custom notes per item
- Let me add custom items not on my master list (either for one job or permanently to the master list)
- Archive completed jobs to a separate tab, with restore and delete options
- A button to publish the job to Google Calendar as an all-day event spanning pickup → return date, titled "Client - Job Name - Rental", with a link to the hosted app in the event body
- Save all state to localStorage so it persists between sessions
- Work well on mobile

Design should be clean and minimal — white cards, light gray background, dark active states. No frameworks or external dependencies.

After building it, tell me how to host it on GitHub Pages.
```

---

## Hosting on GitHub Pages

1. Create a free account at [github.com](https://github.com)
2. Create a new public repository
3. Upload the HTML file Claude gives you — rename it `index.html`
4. Go to **Settings → Pages → Source: Deploy from branch → main / root → Save**
5. Your app will be live at `https://yourusername.github.io/your-repo-name` within a minute

Add it to your phone's home screen: in Safari tap Share → Add to Home Screen. On Android use the browser menu.

---

## Updating

When Claude builds you a new version with improvements, just upload the new `index.html` to your repo and it'll go live automatically in about 60 seconds.

---

*Built by Mercantile Images, LLC · trevrmerchant.com*
