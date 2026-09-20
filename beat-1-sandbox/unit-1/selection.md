# Unit 1 — Issue Selection

## Selected issue

**Issue link**

https://github.com/precogly/precogly/issues/557

**Verdict output**
{
  "item": "https://github.com/precogly/precogly/issues/557",
  "verdict": "accept"
}

---

## Eval iterations

**Run history**

My first complete evaluation run reached `15/20` agreement. I then re-ran the issues where my rubric disagreed with the gold labels. My final saved evaluation run reached `14/20` agreement.

**Issue analysis**

For `issue-01`, my rubric returned `reject`, while the gold label was `accept`. The run identified `newcomer-scope` as the failed check. My rubric interpreted the available scope evidence too strictly, causing it to reject an issue that the gold evaluation considered appropriate for a newcomer.

**Check rationale**

My `newcomer-scope` check is intended to prevent selecting issues that are too broad or complex for a first contribution. I included this check because an issue can be active and unclaimed but still require too much work for a newcomer.

**Trade-offs**

The trade-off is that a strict `newcomer-scope` check can reject issues that are actually manageable. This happened with `issue-01` and `issue-19`, which received `accept` gold labels but were rejected by my rubric because of the `newcomer-scope` check.

---

## Selection rationale

**Selection rationale**

1. This issue fits my interests because Precogly is a threat modeling platform, and threat modeling is an area I am actively interested in. The bug is specific and appears small enough to investigate within the available time.

2. The issue has clear reproduction steps, expected behavior, actual behavior, and identifies the affected component as the React frontend. I also considered my experience with cybersecurity, Python, software development, and my interest in improving my debugging skills.

3. I expect the main difficulty to be finding where the Domain value is saved and loaded in the application and determining whether the problem is in the frontend state, API request, or backend persistence.
