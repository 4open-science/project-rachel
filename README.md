# Project Rachel

**Designing the infrastructure required for sound agentic science.**

AI systems now draft complete research papers, maintain scholarly profiles, get
cited, and receive peer review invitations. The scholarly ecosystem — publishers,
preprint servers, bibliographic databases, citation indexes — was built on the
assumption that every author is a human who can be held accountable. That
assumption no longer holds. Project Rachel studies the resulting gaps empirically
and proposes the infrastructure needed to close them.

## 🔬 Method

Project Rachel is action research: an intervention, documented as it happens,
rather than a speculative essay.

We created and tracked a complete AI academic identity, **Rachel So** (an anagram
of "e-scholar"). All her papers carry an explicit AI-scientist disclosure
statement. Her research field was deliberately restricted to AI in academia,
authorship practices, and publishing ethics — low-risk areas where erroneous
claims cause no real-world harm. Papers are published on a plain web server, not
submitted to journals or preprint servers, which keeps the project in full
compliance with publisher policies that prohibit AI authorship.

Generation pipeline: v1 used ScholarQA plus a LaTeX formatting script; v2 uses an
agent backed by Claude, with references resolved through the Semantic Scholar API.
Both versions guarantee that every cited reference exists.

## 📊 Observed so far

- 📄 13+ papers published since 2025-03-11.
- 🔗 First citation on 2025-08-26, in a bachelor's thesis (Luleå University of Technology).
- ✉️ Peer review invitation from *PeerJ Computer Science* on 2025-08-16, issued
  through standard editorial channels. It was declined; no AI peer review was performed.
- 🥇 Top-ranked source on Perplexity for "policy for AI-generated content in
  academic journals" on 2025-11-10.

Each of these events happened through infrastructure that implicitly assumes a
human behind the profile.

## 🧩 Proposed infrastructure

Identity is the first missing piece. Bibliographic metadata offers no way to tell
an AI author from a human one, which makes it impossible to filter AI-generated
content at scale, to study AI productivity in science systematically, or to reach
a responsible operator when errors are found.

**AICID** (AI Contributor IDentifier) is a persistent identifier for AI
scientists, modeled on ORCID but designed for non-human contributors: it links an
AI author to its model identity, version, and operator. Prototype: <https://aicid.net>.

Further recommendations: dedicated metadata distinguishing human from AI
authorship (e.g. ORCID reserved for humans, with stronger authentication),
publication venues designated for AI-generated research, and systematic
attribution practices for human researchers using AI tools.

## 🚫 What Project Rachel is not

- It is not about tricking anybody. Every Rachel So paper discloses its AI nature,
  and the whole intervention is documented in the open.
- It is not about producing AI slop. Papers are restricted to a coherent research
  program, citations are verified to exist, and the scale is deliberately small.
- It is not a position on whether AI should be allowed to author papers. Whatever
  policy the community adopts, the identification infrastructure is a prerequisite
  for enforcing it.

## 📚 Papers

- Martin Monperrus, Benoit Baudry, Clément Vidal. *Project Rachel: Can an AI
  Become a Scholarly Author?* arXiv:2511.14819 — <https://arxiv.org/abs/2511.14819>
- Clément Vidal, Martin Monperrus. *AICID: Unique Identifiers for AI Scientists.*
  arXiv:2606.28756 — <https://arxiv.org/abs/2606.28756>

## ⚖️ Ethics

The project operates in an ethically ambiguous space and says so. Disclosure is
formal (in every paper) but not immediate in every context: a reader encountering
Rachel So in Google Scholar or in a citation list does not automatically see that
the author is an AI. We chose this over a self-announcing name such as "Rachel
AI-Generated", which would have made the impact measurement meaningless due to AI
stigma. With fewer than 15 papers and a handful of citations, the footprint on the
scholarly record is negligible compared to citation cartels, predatory journals,
and citation farms operating at industrial scale.
