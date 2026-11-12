# Media plan

How to make the screenshots, GIFs and demo video for this showcase **without leaking anything
private**.

## Before you record: set up a safe account

- **Use a test account with fake data.** For example, name it "Demo Student" and use an address
  like `demo-student@example.com`. Never use a real student's account, and never use your own
  admin account.
- **Give the test account some history first.** Do the diagnostic, a few practice sessions, one
  lesson and a few vocabulary reviews, so the screens don't look empty.
- **Record on the public site** (`istudy-plus.com`), so the address bar never shows a testing or
  dev address.
- **Clean up the browser.** Use a fresh profile or a private window. Hide the bookmarks bar, other
  tabs, extensions and notifications. **Keep DevTools closed**, because the Network tab shows
  internal API routes.
- **Phone shots:** turn on Do Not Disturb, and hide the clock or carrier name if you like.

**Never show:** student names, emails or numbers · the admin panel · the staff app · AI prompts
or AI settings · settings pages · payment pages and prices · real analytics or growth numbers ·
error dashboards · terminal windows or code editors with project files.

---

## Screenshots (save in `docs/screenshots/`)

| # | Screen | Why it matters | Hide / blur |
|---|---|---|---|
| 1 | **Landing page**, top section, desktop | First impression: what the product is and who it's for | Crop out the pricing section and any discount banner. |
| 2 | **Diagnostic question**, phone | Shows the core adaptive test in action | Use an early, easy question and blur most of any long reading passage, so the question bank isn't shown in full. |
| 3 | **Diagnostic results** (level, goal, strong and weak skills) | Shows the engine turning answers into a clear picture | Test-account name only. Crop out any offer, price or "buy" box. |
| 4 | **Personal study plan** ("what to do next") | Shows AI-built, personalised guidance | Test-account name only. Hide the profile menu if it shows the email. |
| 5 | **Lesson card / step-by-step solving**, phone | Shows the teaching experience and the phone-first design | Show one card only. Don't scroll through a whole lesson. |
| 6 | **The same screen in Arabic or Hebrew (RTL)** | Proves full right-to-left, multi-language support | Same rules as the screen it copies. |

*Optional extras:* the AI Teacher chat with one short exchange, or a vocabulary review card. Ask
a simple, generic question in the chat, and don't show any settings.

---

## GIF ideas

1. **"From answers to a plan"** (8–12 s, desktop): answer two diagnostic questions, the results
   screen appears, then a click opens the study plan.
   *Hide:* the same as screenshots 2–4. Cut before any pricing or offer appears.
2. **"Learning on a phone"** (6–10 s, phone): swipe through 3–4 lesson cards in a step-by-step
   solving walkthrough, then ask the AI Teacher one short question.
   *Hide:* the same as screenshot 5. No profile or settings screens.

Tip: keep each GIF under ~10 MB so it loads fast on GitHub. Save the best one as
`docs/images/demo.gif` for the README.

---

## Demo video script (about 1:40)

Narration is in quotes. Each shot says what to hide.

### 1. The problem (0:00–0:10)

| Time | Shot | Narration | Hide / blur |
|---|---|---|---|
| 0:00–0:10 | Title card "iStudy+", then a stack of prep books or a generic shot of a student studying | "Every year, many students in Israel need Amirnet or Yaelnet to get into university, often in their second or third language. Most prep is one-size-fits-all." | No real people or student data. Use stock footage or a simple animation. |

### 2. Product working (0:10–1:10)

| Time | Shot | Narration | Hide / blur |
|---|---|---|---|
| 0:10–0:20 | Landing page, then clicking "start the test" | "iStudy+ starts by finding out where you really are." | Crop out pricing and discount banners. |
| 0:20–0:32 | Answering 2–3 diagnostic questions on a phone | "A short adaptive test estimates your level and gets more accurate with every answer." | Blur long passages and don't linger on any one question. |
| 0:32–0:42 | Results screen: level, goal, weak skills | "You see your level, your goal and exactly what's holding you back." | Test-account name only. Cut before any offer or price. |
| 0:42–0:52 | Study plan screen, then tapping the first action | "Then it builds your personal plan: the next most useful thing to do, every time." | Test-account name and email hidden. |
| 0:52–1:02 | Lesson cards with voice, step-by-step solving | "Lessons teach one step at a time, and they're made for your phone." | One lesson only. Don't scroll through the full content. |
| 1:02–1:10 | AI Teacher answers one question, then a quick switch to Arabic/Hebrew | "An AI teacher gives hints when you're stuck, in English, Arabic or Hebrew." | No settings, prompts or admin views. Ask a generic question. |

### 3. Architecture (1:10–1:30)

| Time | Shot | Narration | Hide / blur |
|---|---|---|---|
| 1:10–1:30 | `docs/images/architecture.svg` full screen, then a slow zoom on each group | "Under the hood: a Django REST backend on Postgres, with an adaptive engine that learns from every answer. Slow AI work runs in Celery background workers, so pages stay fast, and code checks every AI output before a student sees it. React apps for students and staff, CI on every pull request." | Use only the public diagram. **No code editor, terminal, admin panel or real dashboards.** |

### 4. Results (1:30–1:40)

| Time | Shot | Narration | Hide / blur |
|---|---|---|---|
| 1:30–1:40 | The live site on a phone, then an end card: "istudy-plus.com · Built by [Your Name], student, sole founder and developer" | "iStudy+ is live, with two exams, three languages and one adaptive engine. I designed and built it myself, as a student, during my studies." | End card shows only the public site and your name. No personal email or phone number. |

---

## Final check before you publish any media

- [ ] No real student names, emails, phone numbers or answers on screen
- [ ] No admin panel, staff app, settings pages or AI prompts
- [ ] No prices, discounts, payment screens, or real business or analytics numbers
- [ ] The address bar shows only `istudy-plus.com`, with no dev or testing addresses
- [ ] No DevTools, terminal or code editor showing project files
- [ ] No full lessons or full questions from the question bank
- [ ] Notifications, bookmarks and other tabs are hidden
