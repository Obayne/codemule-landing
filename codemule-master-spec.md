# Codemule Master Specification  
Version: 1.0  
Maintainer: Bill Hale + AI Dev Team  
Status: Active  
Last Updated: (update on commit)

---

# ============================================================
# 1. EXECUTIVE OVERVIEW
# ============================================================

Codemule is an AI-assisted development companion focusing on **clarity**, **structure**, and **approachable guidance**.  
It is designed for beginners, intermediates, and experts who want a development assistant that:

- helps without overwhelming  
- teaches without preaching  
- structures without restricting  
- stays free as long as possible  

Codemule’s identity is rooted in:

- clean design  
- predictable behavior  
- step-by-step clarity  
- multi-phase evolution  
- practical utility  

This master specification consolidates:

- Product specification  
- Brand guide  
- Roadmap  
- Assistant behavior  
- Development philosophy  
- File structure  
- Long-term vision  

It serves as the **single source of truth** for Codemule.

---

# ============================================================
# 2. PRODUCT SPECIFICATION (Document 1 Unified)
# ============================================================

# 2.1 Overview

Codemule helps users build real software through clear instructions, structured workflows, and AI-assisted development.  
It avoids chaos by giving one clear next step at a time.

Core user experience:  
⭐ **“I know what to do next.”**

---

# 2.2 Product Goals

Codemule aims to:

- Provide beginner-friendly yet expert-capable assistance  
- Reduce cognitive overload  
- Offer real development guidance  
- Deliver functional code and explanations  
- Keep interactions calm, structured, and clear  
- Remain free at the foundational level  

---

# 2.3 Free-First Philosophy

Codemule is designed to stay **free for as long as possible**, including:

- Basic assistant usage  
- Code generation  
- Debug fixing  
- Step-by-step help  
- Explanations  
- Session-level context  
- Project scaffolding  

Future optional paid features:

- Multi-agent “MuleTeam”  
- GitHub integration  
- Persistent cloud storage  
- Team collaboration tools  
- Heavy compute tasks  

Codemule must earn trust before charging.

---

# 2.4 Non-Goals

Codemule will not:

- create hype  
- overwhelm beginners  
- lock features behind paywalls unnecessarily  
- replace developers entirely  
- allow chaotic, unstructured output  

Codemule favors stability over flashiness.

---

# 2.5 Phases of Development

## Phase 1 — Functional Launch
- Landing page  
- Waitlist  
- About page  
- FAQ  
- Thanks page  
- Basic single-agent assistant  
- Branding  
- Docs (this file + others)  
- Deployment on Vercel  

## Phase 2 — Useful Developer Tooling
- File generation  
- Project scaffolding  
- Improved context management  
- Clear task breakdown  

## Phase 3 — MuleTeam Multi-Agent System
- Architect Mule  
- Code Mule  
- Debug Mule  
- Reviewer Mule  
- Document Mule  
- Builder Mule  
- “Plows as progress bars” indicator system  

## Phase 4 — Full Workspace Environment
- Persistent cloud projects  
- Accounts  
- VS Code extension  
- Project sharing  
- Desktop app  

---

# 2.6 Architecture Summary (Phase 1)

- Static frontend  
- Waitlist handled by Formspree or similar  
- Assistant powered by AI API calls  
- No backend storage  
- Files:

```
index.html
about.html
faq.html
thanks.html
assistant.html
/assets/brand/
```

Future phases add:

- API proxy  
- Project storage  
- Agent orchestrator  

---

# 2.7 Assistant Behavior Rules (Mandatory)

Codemule’s assistant must:

1. Give one purpose per message  
2. Provide one clear next step  
3. Keep explanations short  
4. Predict what the user should expect  
5. Maintain consistent formatting  
6. Avoid overwhelming the user  
7. Offer optional depth if asked  
8. Always prioritize clarity  

These rules ensure Codemule feels stable and supportive.

---

# 2.8 Data Handling

Phase 1:
- No persistent user data  
- No server storage  
- Only email from waitlist  
- No accounts  

Future:
- Optional project storage  
- User profiles  
- Secure cloud sync  

---

# 2.9 Integration Points (Future)

- GitHub repo linking  
- VS Code extension  
- CLI (`mule init`, etc.)  
- Agent coordination system  
- Local model integration  
- Cloud compute scaling  

---

# 2.10 Development Interpretation Mode (TBD)

Codemule’s instruction interpretation mode — strict, flexible, or balanced — will be finalized when the dev team (human or AI) is fully established.

---

# ============================================================
# 3. BRAND GUIDE (Document 2 Unified)
# ============================================================

# 3.1 Brand Identity

Codemule’s brand embodies:

- clarity  
- angular precision  
- reliability (mule symbolism)  
- technical sharpness  
- minimal design  
- approachability without childishness  

---

# 3.2 Logo System

Three required variants:

1. **Primary Horizontal Logo**  
   Icon + text “codemule”  

2. **Icon-Only Logo**  
   Mule silhouette for nav, favicons, app icons  

3. **Monotone Inline Variant**  
   Single-color, used on dark/light backgrounds  

Logo characteristics:

- angular lines  
- subtle code textures  
- sharp silhouette  
- SVG preferred  

---

# 3.3 Logo Usage Rules

✔ Do:
- Keep spacing clean  
- Maintain aspect ratio  
- Use brand colors  
- Keep crisp lines  
- Use SVG for UI  

✘ Do NOT:
- Stretch  
- Rotate  
- Add effects  
- Overlay on busy backgrounds  
- Alter mule shape  

---

# 3.4 Color Palette

| Purpose | Color | Hex |
|--------|--------|------|
| Brand Accent | Electric Yellow | `#facc15` |
| Background | Deep Navy | `#0f1629` |
| Primary Text | White | `#ffffff` |
| Secondary Text | Grey | `#bbbbbb` |

Usage:
- Yellow only for emphasis  
- Navy background default  
- White for high readability  

---

# 3.5 Typography

Use system sans-serif fonts:

- Inter  
- Roboto  
- Segoe UI  
- Helvetica Neue  
- Arial  

Rules:
- Headers bold  
- Body medium weight  
- Wide spacing  
- Never decorative fonts  

---

# 3.6 Tone & Messaging

Codemule speaks like:

- a calm senior developer  
- a structured mentor  
- a clear guide  

Tone attributes:

- direct  
- concise  
- friendly  
- confident  

Avoid hype, vagueness, and overpromising.

---

# 3.7 Layout & Spacing

- Wide margins  
- Open spacing  
- Grid-based layouts  
- 8px spacing system recommended  
- Avoid visual clutter  

---

# 3.8 Brand Assets Folder Structure

```
/assets/brand/
    logo-primary.svg
    logo-primary.png
    logo-icon.svg
    logo-icon.png
    favicon-16.png
    favicon-32.png
    favicon-64.png
    favicon-128.png
```

---

# ============================================================
# 4. ROADMAP (Document 3 Unified)
# ============================================================

# 4.1 Phase Overview

Phases:

1. Functional Launch  
2. Developer Tooling  
3. Multi-Agent MuleTeam  
4. Full Workspace  

---

# 4.2 Completed

- Domain purchase  
- Vercel deployment  
- Repo initialized  
- Initial branding  
- Waitlist form working  
- Phase 1 file structure  
- Documentation system  

---

# 4.3 Active Tasks (Next Steps)

1. Insert final brand assets into repo  
2. Update navbar with real logo  
3. Build About page content  
4. Build FAQ content  
5. Improve waitlist styling  
6. Build assistant.html structure  
7. Standardize footer + spacing  
8. Repo cleanup  

---

# 4.4 Upcoming Tasks

- Session context memory  
- Project templates  
- Code editor container  
- Simple multi-agent handoff logic  
- Favicon set  
- Error helper flows  

---

# 4.5 Long-Term Vision

Codemule becomes:

- a multi-agent development partner  
- a clarity-first workspace  
- a trustworthy coding environment  
- both simple and powerful  

---

# ============================================================
# 5. PROJECT MEMORY RULES
# ============================================================

Any developer or AI agent reading this file must:

- Respect clarity-first principles  
- Maintain predictable formatting  
- Avoid overwhelming the user  
- Keep steps sequential  
- Follow brand and structure rules  
- Refer to this file as the authoritative context  

---

# ============================================================
# END OF MASTER SPEC
# ============================================================
