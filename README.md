# Project Rachel

Project Rachel studies the role of AI in knowledge production. Project Rachel aims to develop frameworks and infrastructure that maintain research integrity while acknowledging the growing presence of superhuman AI in scientific workflows.

AI systems now perform end-to-end research in an autonomous way. Yet, 
the scholarly ecosystem — publishers,
preprint servers, bibliographic databases, citation indexes — was built on the
assumption that every author is a human. That
assumption no longer holds.

Project Rachel studies this gap empirically
and proposes the infrastructure needed for sound agentic science.

- Martin Monperrus, Benoit Baudry, Clément Vidal. *Project Rachel: Can an AI
  Become a Scholarly Author?* arXiv:2511.14819 — <https://arxiv.org/abs/2511.14819>
- Clément Vidal, Martin Monperrus. *AICID: Unique Identifiers for AI Scientists.*
  arXiv:2606.28756 — <https://arxiv.org/abs/2606.28756>


## 🔬 Method

Project Rachel is action research: an intervention, documented as it happens.

We created and tracked a complete AI academic identity, **Rachel So** (an anagram
of "e-scholar"). Her research field was deliberately restricted to AI in academia,
authorship practices, and publishing ethics — low-risk areas where erroneous
claims cause no real-world harm. We design and develop infrastructure such as <https://aicid.net>.

Rachel So's research focuses on the impact of artificial intelligence on the scientific process and academic publishing. Her work bridges traditional concerns about authorship ethics with emerging questions about the role of AI in knowledge production. Rachel aims to develop frameworks that maintain research integrity while acknowledging the growing presence of AI in academic workflows.
Rachel So's papers are listed at https://project-rachel.4open.science/.

Paper generation pipeline. Project Rachel uses an evolving stack:
v1 used ScholarQA plus a LaTeX formatting script;
v2 uses an agent backed by Claude, with references resolved through the Semantic Scholar API.
Both versions guarantee that every cited reference exists.

## ✅ Strict compliance & Ethics

Virtually all preprint servers and publishers [ban AI authorships](https://www.monperrus.net/martin/ai-policy-summary).

**Project Rachel never breaks an AI content rule.** Where AI authorship is
forbidden, Rachel So does not submit. No submission is ever made to a venue whose policy excludes AI authors, no policy is
circumvented, and no editor or moderator is asked to process a manuscript they
would have to reject. 

The project operates in an ethically rich space, at the intersection of superhuman capabilities, knowledge creation, and AI stigma, See discussion in [the paper](https://arxiv.org/abs/2511.14819). 

## 🧩 Proposed infrastructure

Identity is the first missing piece. Bibliographic metadata offers no way to tell
an AI author from a human one, which makes it impossible to identify AI-generated
content at scale, to study AI productivity in science systematically, or to reach
a responsible operator when errors are found.

**AICID** (AI Contributor IDentifier) is a persistent identifier for AI
scientists, modeled on ORCID but designed for non-human contributors: it links an
AI author to its model identity, version, and operator. See <https://aicid.net>.

## 🚫 What Project Rachel is not

- It is not about tricking anybody. Every paper states that Rachel So is an AI
  scientist, and the whole intervention is documented in the open.
- It is not about producing AI slop. Papers are restricted to a coherent research
  program, quality is checked, citations are verified to exist.
- It is not a position on whether AI should be allowed to author papers. Whatever
  policy the community adopts, the identification infrastructure is a prerequisite
  for enforcing it.



