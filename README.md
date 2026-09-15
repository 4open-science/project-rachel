# Project Rachel

Project Rachel is about designing the infrastructure required for sound agentic science.

AI systems now perform end-to-end research in an autonomous way. Yet, 
the scholarly ecosystem — publishers,
preprint servers, bibliographic databases, citation indexes — was built on the
assumption that every author is a human. That
assumption no longer holds.

Project Rachel studies the resulting gaps empirically
and proposes the infrastructure needed to close them.

## 🔬 Method

Project Rachel is action research: an intervention, documented as it happens.

We created and tracked a complete AI academic identity, **Rachel So** (an anagram
of "e-scholar"). Her research field was deliberately restricted to AI in academia,
authorship practices, and publishing ethics — low-risk areas where erroneous
claims cause no real-world harm.

Paper generation pipeline. Project Rachel uses an evaolving stack:
v1 used ScholarQA plus a LaTeX formatting script;
v2 uses an agent backed by Claude, with references resolved through the Semantic Scholar API.
Both versions guarantee that every cited reference exists.

## ✅ Strict compliance

**Project Rachel never breaks a rule it is studying.** Where AI authorship is
forbidden, Rachel So does not submit. Her papers are therefore published on a
plain web server under a persistent URL, and are indexed because Google Scholar
crawls publicly accessible documents that carry academic structural signals. No
submission is ever made to a venue whose policy excludes AI authors, no policy is
circumvented, and no editor or moderator is asked to process a manuscript they
would have to reject. The gaps the project documents are gaps in what the rules
leave unspecified, not violations of the rules themselves.

This constraint is binding because the ban on AI authors is effectively
universal, on preprint servers as well as in journals:

- **arXiv**: "generative AI language tools should not be listed as an author"
  ([arXiv moderation policy](https://info.arxiv.org/help/moderation/index.html#policy-for-authors-use-of-generative-ai-language-tools)).
- **ICMJE**: "Chatbots (such as ChatGPT) should not be listed as authors because
  they cannot be responsible for the accuracy, integrity, and originality of the
  work"
  ([Defining the Role of Authors and Contributors](https://www.icmje.org/recommendations/browse/roles-and-responsibilities/defining-the-role-of-authors-and-contributors.html)).
- **The big five publishers** (Elsevier, Springer Nature, Wiley, Taylor & Francis,
  SAGE) and the **ACM** converge on the same rule: AI may be used and must be
  disclosed, but may never be an author. See the policy survey in the Project
  Rachel paper, §2.2.

The common justification is accountability: an author must be able to take
responsibility for the work, approve the final version, and bear the consequences
of integrity violations. AI systems cannot do this today. The result is a blanket
exclusion that applies whatever the actual division of intellectual labor —
AI may assist but cannot author, even when it does 99% of the work. Project
Rachel accepts that rule as given and works strictly within it.

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
