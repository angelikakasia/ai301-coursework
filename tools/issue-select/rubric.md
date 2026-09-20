# Rubric: is this a good first issue?

<!--
THIS IS THE PART YOU WRITE. The skill in SKILL.md executes whatever checks
you define here. It ships empty on purpose: the judgment is your work.

A filled rubric must contain:

1. At least one row in the checks table. Each row needs all four columns:
   - Check: a short name (used in the output JSON).
   - Evidence: exactly what to look at, and where. Name the source
     (repo-facts block, issue body, comment thread, or the locations in
     references/evidence-guide.md). "The repo" is not a source; "the last
     5 default-branch commit dates" is.
   - Pass condition: a condition someone else could apply and get your
     answer. Prefer thresholds with numbers ("a maintainer commented
     within 30 days") over adjectives ("maintainer is responsive").
   - Weight: `required` (a fail here rejects the issue) or `preferred`
     (never changes the verdict; a nice-to-have that helps rank the
     issues you accept).

2. A verdict rule below the table: how the check grades combine into
   accept or reject, including how `unclear` is treated. The verdict
   space is binary. If you write no rule for `unclear`, the skill treats
   it as fail.

Cover what actually kills first contributions. The lecture named four
families: the maintainer is alive, the repo is in use, the scope fits a
newcomer, and nobody else is already on it. A rubric that ignores a family
will fail eval issues designed around that family.
-->
## Checks

| Check | Evidence | Pass condition | Weight |
|---|---|---|---|
| maintainer-alive | Comment thread and the maintainer activity locations listed in references/evidence-guide.md | Pass if a maintainer has shown activity within the last 90 days. | required |
| repo-active | Repo-facts block and the last 5 default-branch commit dates | Pass if the repository has at least one default-branch commit within the last 90 days. | required |
| newcomer-scope | Issue body and comment thread | Pass if the issue describes a specific problem or requested change and does not explicitly require a large architectural rewrite or broad multi-component change. | required |
| unclaimed | Issue body and comment thread | Pass if there is no clear statement that another contributor is currently working on the issue. | required |
| clear-guidance | Issue body | Pass if the issue provides enough information to identify the problem, expected behavior, or requested change. | preferred |

## Verdict rule

Accept if every required check passes. Reject if any required check fails. An unclear result on a required check counts as fail. Preferred checks do not change the accept or reject verdict and are used only to rank accepted issues.
<!-- State how the grades above combine into accept or reject, and how
unclear is treated. Example shape (write your own): "accept if every
required check passes; preferred checks never change the verdict, they
rank accepted issues; unclear counts as fail." -->
