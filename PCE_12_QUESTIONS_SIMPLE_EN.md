# PCE — The 12 Questions, Simple English + Wisdom

> **How to use this file:**
> Part 1 taught you the **blocks** (FATP, CIA, DCVC, AER, MPD, MEA). See [PCE_BLOCKS_SIMPLE_EN.md](PCE_BLOCKS_SIMPLE_EN.md).
> This file walks through **each of the 12 questions**: what it really asks in plain words, the hard English words explained, and the **wisdom** = how to build the answer fast.
> **Big rule again:** marks come from *points*, not perfect words. Bullet points + 1 example = full marks.

---

## ⚡ Speed map — which block answers which question
| Question topic | Trigger word | Block to use |
|---|---|---|
| Q1 importance of IT ethics | "ethics / why important" | examples only |
| Q2 four data-science principles | "principles" | **FATP** |
| Q3 framework vs regulation | "should vs must" | *(no block — see below)* |
| Q4 algorithmic bias | "bias" | Amazon + COMPAS |
| Q5 why fairness in AI | "fairness" | FATP-F + Golden Rule |
| Q6 GDPR | "GDPR / rights" | **AER** |
| Q7 informed consent | "consent" | **DCVC** |
| Q8 CIA triad | "security goals" | **CIA** |
| Q9 security threats | "threats" | **MPD** |
| Q10 privacy in software | "privacy by design" | **MEA** |
| Q11 explainability | "why AI decided" | *(no block — see below)* |
| Q12 apply PCE in future | "in your career" | mix CIA+MEA+FATP |

---

## Q1 — Why is IT ethics important?
**Hard words:**
- **Ethics** = the study of right and wrong behaviour.
- **Profiling** = building a detailed picture of a person from their data (to judge/predict them).
- **Breach** = a leak / break-in where data is stolen.

**Plain answer:** Technology makes ethical problems bigger and faster. It can spy on people and judge them (profiling).
**3 ready examples:** Facebook–Cambridge Analytica (data misused for politics) · employee monitoring (watching workers) · Equifax breach (huge data leak).
**Why it matters:** for *people* → protects their privacy; for *companies* → keeps trust and avoids lawsuits.

**Wisdom:** Say "tech increases ethical problems" → give 1 example → give 1 effect (person + company). Done.

---

## Q2 — The 4 data-science principles
**This is pure FATP.** Fairness · Accountability · Transparency · Privacy.

**Wisdom:** Write each word + "means..." + 1 example. (See Block 1.) 4 words = 4 points. Easiest question on the paper.

---

## Q3 — Framework vs Regulation ("should" vs "must")
**Hard words:**
- **Framework / guideline** = advice you *should* follow, but it's **voluntary** (no police). Example: **ACM Code of Ethics**. Key word = **should**.
- **Regulation** = a real **law** you **must** obey or get punished. Examples: **HIPAA** (US health data), **COPPA** (US kids' data), **GDPR** (EU data). Key word = **must**.

**Plain answer:** A framework is advice (should, voluntary). A regulation is law (must, punishment).

**Wisdom:** The whole answer is the contrast: **should vs must**, **voluntary vs law**. Give 1 example of each (ACM Code vs GDPR). 

---

## Q4 — What is algorithmic bias?
**Hard words:**
- **Algorithm** = the step-by-step rules a computer follows to decide.
- **Bias** = unfair leaning toward/against a group.
- **Systematic** = happens again and again in a pattern (not by accident).

**Plain answer:** Algorithmic bias = when an AI gives **unfair, discriminatory results in a repeating pattern**, usually because it learned from **biased data**.
**2 examples:** **Amazon** (AI rejected women) + **COMPAS** (court tool unfair to Black people).

**Wisdom:** Definition (1 line) + the 2 examples. The examples ARE the marks here.

---

## Q5 — Why is fairness important in AI?
**Plain answer:** AI now makes **big life decisions** — jobs, loans, policing. If it's unfair it:
- causes real **harm** to people,
- increases **inequality** (the gap between groups),
- destroys **trust**,
- creates **legal responsibility** (the company can be sued).
Link to the **Golden Rule** (treat others as you'd want to be treated).

**Wisdom:** List the 4 harms as bullets + name Golden Rule. Reuse Amazon as the example.

---

## Q6 — What is GDPR?
**Hard words:**
- **GDPR** = General Data Protection Regulation — the EU's data-protection **law** (from **2018**).

**Plain answer:** A strong EU law that protects people's personal data and gives them rights.
**3 rights = AER:** **Access** (see my data) · **Erasure** (delete it / "right to be forgotten") · **Rectification** (fix wrong info).

**Wisdom:** Name the law (EU, 2018) + the 3 rights. Hook: **See it, Delete it, Fix it.**

---

## Q7 — What is informed consent?
**Hard words:**
- **Informed consent** = the person agreed (said yes) AFTER truly understanding what they agreed to.

**Plain answer:** Getting a real, understanding "yes" **before** collecting someone's data.
**4 elements = DCVC:** Disclosure (told) · Comprehension (understood) · Voluntariness (free choice) · Competence (able to decide).
**Examples:** cookie opt-in on a website, medical consent form.

**Wisdom:** Definition + the 4 DCVC words + 1 example (cookies). Hook: "told → understood → free → able."

---

## Q8 — What is the CIA Triad?
**This is pure CIA.**
- **Confidentiality** = keep secret → protected by **encryption**.
- **Integrity** = data stays correct/unchanged → protected by **hashing**.
- **Availability** = usable when needed → protected by **backup**.
- The threat to Availability = **DoS**.

**Wisdom:** 3 words + how each is protected. Reuse encryption from Q10, reuse DoS from Q9. Three answers in one study session.

---

## Q9 — What are the main security threats?
**This is pure MPD.**
- **Malware** = bad software (Virus / Worm / Trojan).
- **Phishing / spoofing** = fake message pretending to be someone you trust, to steal info.
- **DoS / DDoS** = flooding a system so it stops working.

**Wisdom:** 3 threats + 1 example each. The DoS here is the same one that attacks Availability in Q8 — reuse it.

---

## Q10 — Why does privacy matter in software?
**Hard words:**
- **Identity theft** = a criminal steals your personal info to pretend to be you.
- **Privacy by design** = build privacy INTO the software from the start, not added later.

**Plain answer:** Privacy matters because weak software leads to identity theft and breaks the law. Good software uses "privacy by design".
**3 practices = MEA:** Minimisation (collect less) · Encryption (scramble it) · Access control (limit who enters).

**Wisdom:** Say why (identity theft + law) → "privacy by design" → list MEA. Encryption reused from Q8.

---

## Q11 — What is explainability?
**Hard words:**
- **Explainability** = being able to understand and explain **WHY** an AI made its decision.
- **Black box** = a system where you see the input and output but NOT how it decided inside.

**Plain answer:** Explainability = the AI can show **why** it decided, instead of being a mystery (black box).
**Why it matters:** accountability (someone can be answerable), finding bias, building trust, and GDPR requires it.
**Example:** a loan is refused → the system must say "because your income is too low," not just "no."

**Wisdom:** Define it against "black box" → 3–4 reasons it matters → the loan example.

---

## Q12 — How will you apply PCE in your future career?
**PCE** = Professional Computing Ethics (the subject itself).
**Plain answer — give 3 actions:**
1. **Privacy & security by design** from the start (use **MEA** + **CIA**).
2. **Test for fairness / bias** in my systems (remember **Amazon**).
3. **Use ethical principles when stuck** — **Laudon principles** + **ACM Code of Ethics**.

**Wisdom:** This question lets you reuse EVERYTHING. Just pick 3 actions, each pointing to a block you already know.

---

## 🧠 Final wisdom for the 12 questions
1. **One trigger word** in the question tells you which block to grab (see the Speed map at top).
2. Many questions **share answers** — CIA/encryption (Q8, Q10, Q12), FATP/fairness/bias (Q2, Q4, Q5, Q12), Amazon+COMPAS (Q4, Q5). Learn once, answer many.
3. Build every answer the same way: **definition → block words → 1 example.**
4. **Bullet points, not essays.** Points = marks.
5. **Read aloud** when studying — it sticks better than silent reading.

**Truth:** It looks like 12 questions, but it's really only ~6–7 things to learn. Master the blocks and the answers write themselves.
