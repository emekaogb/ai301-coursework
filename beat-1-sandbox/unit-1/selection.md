# Unit 1 — Issue Selection

Path: `beat-1-sandbox/unit-1/selection.md`

Record of the issue carried into Unit 2, and of the evaluation runs that produced
`eval-run.txt`. This file is graded at the path above; a copy kept anywhere else in
the repository is not read.

Complete every labelled field below. Each is graded on its own; content placed under the
wrong label is not graded.

---

## Selected issue

**Issue link**

https://github.com/codepath/pathreview-ai301-fa26-s3/issues/71

**Verdict output**

```
Issue #71 Evaluation

  ┌──────────────┬───────┬─────────────────────────────────────────────────────────────────────────────────────────┐
  │    Check     │ Grade │                                        Evidence                                         │
  ├──────────────┼───────┼─────────────────────────────────────────────────────────────────────────────────────────┤
  │ Maintainer     │ pass  │ Repository shows maintainer activity within 180 days (commits dated 2026-09-16 and    │
  │ activity       │       │ earlier)                                                                              │
  ├────────────────┼───────┼───────────────────────────────────────────────────────────────────────────────────────┤
  │ Repository     │ pass  │ Multiple commits in September 2026 on default branch within 180 days                  │
  │ activity       │       │                                                                                       │
  ├────────────────┼───────┼───────────────────────────────────────────────────────────────────────────────────────┤
  │                │       │ Concrete outcome: remove indentation from test fixture in                             │
  │ Newcomer scope │ pass  │ test_extract_heading_hierarchy; identifies tests/unit/test_readme_parser.py and       │
  │                │       │ ingestion/parsers/readme_parser.py; estimated 1–2 hours                               │
  ├────────────────┼───────┼───────────────────────────────────────────────────────────────────────────────────────┤
  │ Issue clarity  │ pass  │ Clearly explains the problem: indentation causes Markdown to treat fixture as code    │
  │                │       │ block, preventing heading extraction                                                  │
  ├────────────────┼───────┼───────────────────────────────────────────────────────────────────────────────────────┤
  │ Existing       │ pass  │ No assignees, no comments or claims; issue is unclaimed                               │
  │ ownership      │       │                                                                                       │
  ├────────────────┼───────┼───────────────────────────────────────────────────────────────────────────────────────┤
  │ Contribution   │ pass  │ docs/CONTRIBUTING.md permits this work type; no AI restriction                        │
  │ policy         │       │                                                                                       │
  ├────────────────┼───────┼───────────────────────────────────────────────────────────────────────────────────────┤
  │ Contribution   │ pass  │ Task is a test fixture formatting fix; uses existing code and tests; no special       │
  │ fit            │       │ infrastructure                                                                        │
  └────────────────┴───────┴───────────────────────────────────────────────────────────────────────────────────────┘

  [
    {
      "item": "https://github.com/codepath/pathreview-ai301-fa26-s3/issues/71",
      "checks": [
        {"name": "Maintainer activity", "grade": "pass", "evidence": "Commits from maintainer dated 2026-09-16, within 
  180 days"},
        {"name": "Repository activity", "grade": "pass", "evidence": "Multiple commits in September 2026 on default 
  branch within 180 days"},
        {"name": "Newcomer scope", "grade": "pass", "evidence": "Concrete task: remove indentation from 
  test_extract_heading_hierarchy fixture; identifies test file and parser file; 1–2 hour estimate"},
        {"name": "Issue clarity", "grade": "pass", "evidence": "Explains problem clearly: indentation makes Markdown 
  treat fixture as code block, preventing heading detection"},
        {"name": "Existing ownership", "grade": "pass", "evidence": "No assignees or comments; issue is completely 
  unclaimed"},
        {"name": "Contribution policy", "grade": "pass", "evidence": "docs/CONTRIBUTING.md permits this work type; no 
  AI ban"},
        {"name": "Contribution fit", "grade": "pass", "evidence": "Test fixture formatting uses existing code and 
  tests; no private infrastructure"}
      ],
      "verdict": "accept"
    }
  ]
```

---

## Eval iterations

Quote source text directly in each field below. Paraphrase does not satisfy them.

**Run history**

Run #1: agreement: 18/20 scored items  (bar: 18/20: PASS)

**Issue analysis**

`issue-01` (conda docs: add PyPI installation guide) has gold label **accept**, but my rubric initially returned **reject**. The problem was my **Newcomer scope** check — it treated multi-file tasks as too large. However, this is a bounded, coherent documentation task with clear deliverables, not an unbounded umbrella issue. I revised the check to focus on whether the issue has concrete scope and a clear outcome, rather than penalizing multiple files.

**Check rationale**

| Repository activity | The repo-facts block showing default-branch commit history and repository activity | Pass if the default branch has at least 3 commits within the last 180 days, or the repository otherwise has documented recent development activity. Fail if there is no documented development activity within the last 180 days. | required |

I included this check because a good first issue should come from an actively maintained repository. Recent default-branch commits provide objective evidence that development is still happening and that contributions are more likely to receive review. The 180-day window gives a reasonable period for measuring recent activity without requiring a project to have extremely frequent commits.

**Trade-offs**

The trade-off of this check is that it may reject repositories that are still maintained but have fewer than three recent default-branch commits. For example, a project could have active issue discussions, releases, or development on other branches without meeting the commit threshold. I accepted this limitation because the goal is to find a first issue in a repository with clear evidence of recent development, and default-branch commits provide a simple and consistent signal for that.

---

## Selection rationale

Graded on whether all three are answered, in your own words. Not on how good the
reasoning is, and not on length — a short honest answer to each earns the full marks.
This is also the basis for the claim comment you write in Unit 2.

**Selection rationale**

**1. Issue fit and time available:**
This issue fits my interests in software engineering and debugging, and the estimated 1–2 hour scope makes it realistic to complete within my available time.

**2. What the verdict identified vs. what I weighed:**
The rubric correctly identified that the issue is clearly scoped and unclaimed. I also considered my own familiarity with Python and testing, which the rubric could not evaluate.

**3. Anticipated difficulty in claiming:**
I expect it to be relatively easy to claim because there is currently no assignee or linked PR, although another contributor could claim it first.


---

Related paths: `eval-run.txt` in this directory; your skill's files in
`tools/issue-select/`.
