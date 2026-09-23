# Rubric: is this a good first issue?

## Checks

| Check | Evidence | Pass condition | Weight |
|---|---|---|---|
| Maintainer activity | The repo-facts block for maintainer activity, including the dates of the most recent default-branch commits and recent maintainer activity described in the issue/comments | Pass if there is at least one documented maintainer activity within the last 180 days. Fail if there is no documented maintainer activity within the last 180 days. | required |
| Repository activity | The repo-facts block showing default-branch commit history and repository activity | Pass if the default branch has at least 3 commits within the last 180 days, or the repository otherwise has documented recent development activity. Fail if there is no documented development activity within the last 180 days. | required |
| Newcomer scope | The issue body, issue comments, and the scope guidance in `references/evidence-guide.md` | Pass if the issue defines a concrete outcome and identifies the main files, components, pages, or areas involved, even when the change spans multiple related files. Fail if the issue is primarily an umbrella/tracking issue, combines many unrelated tasks, calls for a repository-wide or architectural change without a bounded deliverable, or does not define a concrete target. | required |
| Issue clarity | The issue body and comment thread | Pass if the issue identifies a specific problem or desired change and provides enough information to understand what needs to be investigated or changed. Fail if the issue is only a vague request with no identifiable task or problem. | required |
| Existing ownership | The issue body, comment thread, and repository issue/PR evidence described in `references/evidence-guide.md` | Pass if there is no clear evidence that another contributor is currently working on the issue, such as an explicit assignment, claim, active PR, or recent comment stating that someone is working on it. Fail if someone has clearly claimed the issue or an active PR is already addressing it. | required |
| Contribution policy | The repository's contributing guide, code of conduct, developer documentation, and other repository-level contribution-policy files identified in `references/evidence-guide.md` | Pass if the repository's contribution policies permit the type of work required by the issue and do not prohibit the contributor's intended development method. Fail if a repository policy explicitly prohibits completing the issue through the available contribution workflow, including an explicit prohibition on AI-generated code or documentation when AI assistance is being used. | required |
| Contribution fit | The issue body, repository facts, and the locations in `references/evidence-guide.md` relevant to issue scope and contribution status | Pass if the issue can be worked on and validated using the repository's existing code, tests, documentation, and normal development workflow without requiring access to private infrastructure or unavailable resources. | preferred |

## Verdict rule

Accept an issue if every required check passes. Reject an issue if any required check fails. Preferred checks never change the accept/reject verdict and are used only to help rank issues that are accepted. Treat `unclear` as fail for required checks and as a non-passing result for preferred checks.
