# Trace, Tag, Transfer

**A private, interactive exercise for naming the skills no job description names.**

Trace, Tag, Transfer helps you take three skills that hiring reports keep calling essential, **judgment**, **adaptability**, and **clarity from ambiguity**, and connect each one to the real moments in your life where you built it. You finish with three plain-language sentences you can say out loud in an interview, a performance review, or an introduction.

**Live tool:** `https://PinKandPolicY.github.io/trace-tag-transfer/`

---

## The idea

Many people, especially those who have changed countries, careers, or rooms where no one looked like them, carry real expertise they have never been taught to describe. The skills are there, but they live in stories rather than on a résumé.

This tool offers a simple way to bring them into language. It borrows a few ideas from engineering as an analogy (not a formal framework): traceability and debugging, labeling and versioning, and transfer learning.

### How it works

1. **Trace.** Choose a prompt and write one memory about where you built the skill. The memory is for your eyes only.
2. **Tag.** Turn that memory into a single sentence using a simple formula:
   *I [verb] [who or what] so that [result].*
   A level ladder (vague, better, tagged) shows how to sharpen the sentence.
3. **Transfer.** Pick a room you want to be in a year from now, name the problem waiting there for someone like you, and choose which tag you would reach for first.

At the end you get a **card** with your three version 1.0 tags and a closing statement you can copy and keep.

> Your tag does not have to be pretty. It has to run. You can polish it later, like any version 1.0.

---

## Where this comes from

This tool accompanies my presentation **"You wherever You are,"** delivered for the **Capitol Technology University Women in Cyber leadership series** in November 2026. It is an interactive interpretation of the framework I shared in that session, so that attendees, and anyone else, can work through it on their own after the talk.

I created the presentation with Claude Docs.

---

## Built with Claude

I built this tool with Claude, Anthropic's AI assistant, working from my framework and goals. Claude generated the interactive page as a self-contained web artifact, then helped me review it and prepare it for publishing on GitHub Pages. The concept, the framework, the prompts, and the intent are mine. Claude did the heavy lifting on the code, and I directed, reviewed, and edited the result.

---

## Security and design considerations

I work in cybersecurity and governance, so I held this tool to the standard I would ask of any system that touches personal reflection.

### Privacy by design

- **Nothing is saved or sent.** Everything you type stays in your browser tab. There is no server, no database, no account, no login, no cookies, and no analytics. Close the tab and it is gone, which is why the tool prompts you to copy your card first.
- **Memories stay with you.** The page tells users to share only their tag, never the memory behind it. The most personal writing never needs to leave the person who wrote it.
- **Minimal footprint.** The whole tool is one HTML file with no frameworks and no third-party scripts, so there is very little to maintain and very little to exploit.
- **One external request.** The page loads two typefaces (Bricolage Grotesque and Source Sans 3) from Google Fonts. That is the only third-party call. Google receives a standard font request, as with any site that uses hosted fonts, but never anything you type. If the fonts fail to load, the page falls back to your system fonts. Self-hosting the fonts would remove this request entirely.

### Secure coding choices

- **No injection surface.** User input is written to the page as plain text, never as HTML, so what someone types cannot become executable code on the page.
- **No secrets.** The file contains no API keys, tokens, credentials, or personal data, and it makes no calls to any Claude or other API.
- **Graceful clipboard handling.** The "Copy card" button uses the browser's clipboard API and falls back to an older method, with a clear message if copying is blocked.

### Design and accessibility

- **One step at a time.** A short, guided flow keeps the exercise from feeling like a form to fill out.
- **Keyboard and screen reader friendly.** Inputs have labels, the progress rail marks the current step, the live tag preview announces updates, and focus is clearly visible.
- **Responsive and comfortable.** The layout works on phones and desktops, follows the visitor's light or dark preference, and respects reduced-motion settings.
- **Plain language.** The prompts are written to invite honesty rather than performance.

---

## Run it yourself

No build step or installation is needed.

1. Download `index.html`.
2. Open it in any modern browser.

To publish your own copy, upload `index.html` to a GitHub repository and turn on GitHub Pages under **Settings > Pages**.

---

## About the author

Created by **Dee**, founder of **Courageous Daring Wonderful You (CDWY)**, a portfolio venture spanning coaching, consulting, speaking, community building, and the podcast *Bytes, Bits & Brilliance*. Dee is a cybersecurity and IT professional with roughly 28 years of experience, and her work supports underrepresented professionals in tech, particularly women and BIPOC communities.

Connect: [LinkedIn](https://www.linkedin.com/in/dawnbutler1) · [CDWY](https://dawn-butler-portfolio.lovable.app) · [Podcast](https://www.buzzsprout.com/2326005)

---

&copy; 2026 Courageous Daring Wonderful You. All rights reserved.
