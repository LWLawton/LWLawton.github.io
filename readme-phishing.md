# Module 1 — Security Awareness & Phishing Defense

**Dental vCISO Compliance Training Program**  
`phishing-defense.html` · Module 1 of 6 · Compliance Depth

---

## What This Module Covers

A fully self-contained, interactive HIPAA compliance training module covering:

- Why dental practices are targeted by phishers and cybercriminals
- Types of phishing: email, spear, whaling, smishing, vishing, BEC
- How to identify phishing red flags in real dental-practice scenarios
- Social engineering tactics (urgency, authority, reciprocity, social proof)
- What to do when you receive — or accidentally click — a phishing link
- Protection from malicious software *(45 CFR 164.308(a)(5)(B))*
- Login monitoring & password management *(45 CFR 164.308(a)(5)(C)(D))*
- HIPAA breach implications and penalty tiers
- Personal phishing defense checklist

**Regulatory coverage:** 45 CFR 164.308(a)(5) — Security Awareness & Training (Administrative Safeguards)

**Format:** 19 screens · 5 knowledge checks · 100% pass required · Printable PDF certificate

---

## Files in This Module

```
phishing-defense.html        ← Complete standalone training module
README-phishing-defense.md   ← This file
```

---

## How to Open Locally

No build tools, no npm, no dependencies required.

1. Download or clone this repository
2. Open `phishing-defense.html` in any modern web browser
3. Complete the training — all 19 screens and 5 quizzes
4. Print the certificate (Ctrl+P / Cmd+P) and submit to your IT Team Leader

That's it. One file. No server needed.

---

## How to Deploy to GitHub Pages

### Step 1 — Create your repository

```bash
git init dental-vciso-training
cd dental-vciso-training
```

### Step 2 — Add your files

```bash
cp phishing-defense.html ./phishing-defense.html
cp README-phishing-defense.md ./README-phishing-defense.md
git add .
git commit -m "feat: add phishing defense compliance training module"
```

### Step 3 — Push to GitHub

```bash
git remote add origin https://github.com/YOUR-USERNAME/dental-vciso-training.git
git push -u origin main
```

### Step 4 — Enable GitHub Pages

1. Go to your repository on GitHub.com
2. Click **Settings** → **Pages**
3. Under **Source**, select `main` branch and `/ (root)` folder
4. Click **Save**
5. Your module will be live at:  
   `https://YOUR-USERNAME.github.io/dental-vciso-training/phishing-defense.html`

GitHub Pages deployment typically takes 1–3 minutes.

### Step 5 — Automated deployment (optional)

A shared GitHub Actions workflow file is included at:
`.github/workflows/deploy.yml`

This automatically redeploys your site whenever you push changes to the `main` branch.

---

## How to Link from LinkedIn

1. Copy your live GitHub Pages URL:  
   `https://YOUR-USERNAME.github.io/dental-vciso-training/phishing-defense.html`

2. On LinkedIn, go to your **Profile → Featured → Add a link**

3. Paste the URL — LinkedIn will generate a preview card

4. Suggested caption:
   > *"Free HIPAA phishing defense training module I built for dental practices — self-paced, 19 screens, 100% quiz pass required, printable compliance certificate. Part of a 6-module dental vCISO training library."*

5. Also add the repository link to your **Projects** section for hiring managers reviewing your technical work.

---

## For the Practice Owner / IT Team Leader

### What this satisfies

This module, when completed and signed off, contributes to your practice's documented compliance with:

| Regulation | Section | Requirement |
|---|---|---|
| HIPAA Security Rule | 45 CFR 164.308(a)(5)(i) | Security awareness and training program |
| HIPAA Security Rule | 45 CFR 164.308(a)(5)(ii)(B) | Protection from malicious software |
| HIPAA Security Rule | 45 CFR 164.308(a)(5)(ii)(C) | Log-in monitoring |
| HIPAA Security Rule | 45 CFR 164.308(a)(5)(ii)(D) | Password management |

### Record retention

Retain completed, signed certificate PDFs for **a minimum of 6 years** from the date of completion per 45 CFR 164.316(b)(2).

### Recommended training cadence

| Event | Action |
|---|---|
| New hire onboarding | Complete before ePHI access is granted |
| Annual refresh | Repeat every 12 months |
| After any security incident | Mandatory re-completion |
| After role change | Re-complete within 30 days |

---

## Technical Notes for Developers

- **Zero dependencies** — pure HTML, CSS, vanilla JavaScript
- **Quiz data is fully modular** — all questions defined in the `QUIZ_DATA` object at the bottom of the file; logic is completely separate
- **AI enhancement ready** — an `<!-- AI ENHANCEMENT BLOCK -->` comment is included in the JS section where Anthropic API calls can be added via a secure backend proxy
- **Git-diff friendly** — all sections marked with `<!-- SECTION: NAME -->` comments
- **Print-safe** — `@media print` CSS hides all navigation and renders only the certificate
- **Input sanitized** — certificate name field strips non-printable characters and HTML-encodes output before DOM insertion
- **No external requests** — all illustrations are inline SVG; no CDN, no fonts, no tracking

---

## Disclaimer

> This training module is provided for informational and compliance documentation purposes. It does not constitute legal advice. Consult a qualified HIPAA compliance attorney or compliance officer for a formal assessment of your practice's obligations.

---

*Dental vCISO Advisory Services · Built with care for the dental community*
