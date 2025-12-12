# Codemule Technical & Product Specification  
Version: 1.0  
Maintainer: Bill Hale + AI Dev Team  
Status: Active  
Last Updated: (Update upon commit)

---

# 1. OVERVIEW (BEGINNER-FRIENDLY SUMMARY)

Codemule is an AI-powered development assistant designed to help users—from beginners to experts—build real software with clarity, structure, and confidence.  
It is NOT “just another chat interface.”  

Codemule focuses on:

- Real project workflows  
- Clear step-by-step guidance  
- Functional code generation  
- Sustainable architecture  
- Beginner-friendly explanations  
- Expert-level technical depth when needed  
- Reducing mental overload and confusion  

Codemule’s identity is built around **clarity**, **simplicity**, and **real-world usefulness**.

This document explains what Codemule is, how it works, and how it should evolve.

---

# 2. STRUCTURED DETAILS (INTERMEDIATE DEPTH)

## 2.1 Product Goals
Codemule exists to:

- Provide step-by-step coding guidance  
- Generate real working applications  
- Assist with debugging and architecture  
- Help beginners learn without overwhelm  
- Help experts accelerate development  
- Maintain clarity in all outputs  
- Offer structured workflows instead of chaotic chat  

Codemule's core principle:  
**“Clarity > speed. Understanding > shortcuts.”**

---

## 2.2 Core Use Cases
- Building new projects (web, backend, AI, etc.)  
- Improving or refactoring existing code  
- Debugging issues with clear reasoning  
- Technology learning and onboarding  
- Documentation generation  
- Multi-file project scaffolding  
- Architecture planning  

Phase 1 starts simple and grows.

---

## 2.3 Phase Definitions

### Phase 1 — Functional Launch (Current)
- Landing page  
- Waitlist  
- FAQ  
- About page  
- Basic Codemule Assistant (single-agent)  
- Branding + identity  
- Deployment on Vercel  

### Phase 2 — Useful Developer Tool
- Project-based workspaces  
- Simple file editor or generation sandbox  
- Better context management  
- Clear UI for task breakdown  

### Phase 3 — Multi-Agent Dev System
- MuleTeam (coordinated agents)  
- Progress indicators (“plows”)  
- GitHub repository integration  
- CLI tool  
- IDE extensions  

---

## 2.4 Non-Goals (Important)
Codemule does NOT aim to:

- Replace developers entirely  
- Build massive applications autonomously (yet)  
- Include gimmicky visual fluff  
- Overload users with complexity  
- Chase trends  

Codemule must remain **practical, clean, and clarity-first**.

---

## 2.5 Frontend Structure (Phase 1)
Pages:

```
/
|-- index.html
|-- thanks.html
|-- faq.html  (optional merge into index)
|-- about.html
|-- assistant.html   (Phase 1 minimal prototype)
```

Brand assets will live under:

```
/assets/brand/
```

---

## 2.6 Data Flow (Phase 1)
- Waitlist submissions go to a backend service (Formspree temporary → EmailJS or Supabase recommended).  
- No user accounts in Phase 1.  
- No code storage in Phase 1.  
- Assistant interactions are ephemeral unless future storage is added.

---

# 3. DEEP TECHNICAL SPECIFICATION (FOR EXPERTS & AGENTS)

## 3.1 Architecture (Phase 1)
Static frontend deployed on Vercel.  
AI requests originate from client calls to an LLM provider (OpenAI recommended).

No backend server required in Phase 1 except optional:

- API key proxy  
- Request router  
- Custom form handler  

Future phases will introduce server-side logic.

---

## 3.2 Assistant Architecture

### Phase 1 — Single Agent
- Natural language → structured instructions → code outputs  
- Chain-of-thought hidden  
- Minimal context window  
- Accepts explicit instructions from UI  

### Phase 2 — Task Breakdown Engine
Codemule begins to:

- Break tasks into subtasks  
- Show progress markers  
- Maintain ephemeral state  
- Output file trees  

### Phase 3 — MuleTeam (Multi-Agent)
Roles may include:

- Architect Mule  
- Code Mule  
- Debug Mule  
- Document Mule  
- Reviewer Mule  
- Builder Mule  

Communication style:  
**clear, structured, predictable.**

---

## 3.3 Clarity Requirements (IMPORTANT for AI agents)
All AI tools operating within Codemule must follow:

1. One clear purpose per message  
2. One-step-at-a-time guidance  
3. Explanations in one sentence unless asked  
4. Predictable formatting  
5. No info-dumps  
6. No ambiguous steps  
7. Explicit next steps after every major action  

This ensures Codemule remains beginner-friendly while powerful for experts.

---

## 3.4 Data Policies (TBD in Phase 2)
Future spec will define:

- What data Codemule stores  
- How user code is handled  
- Privacy and security model  
- Deletion policies  

For now:  
**Phase 1 stores nothing permanent.**

---

## 3.5 Integration Points
Future integrations:

- GitHub API  
- VS Code extension  
- Local model support  
- Log storage  
- Project scaffolding templates  

---

## 3.6 Development Interpretation Mode (TBD)
Codemule’s instruction interpretation mode—strict, flexible, or balanced—is intentionally **undecided** at this stage.  
To be defined when the dev team (human and/or AI) is formalized.

---

# END OF SPEC

