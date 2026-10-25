# Unit 2 — Claim and Reproduce

## Your identity upstream

**GitHub username**

emekaogb

---

## Posted upstream

**Claim comment**

https://github.com/codepath/pathreview-ai301-fa26-s3/issues/71#issuecomment-6388325255

I'd like to work on this issue. I'll investigate why the indented README fixture produces no headings, reproduce the behavior against the current parser, and share the steps and evidence here. I haven't confirmed the root cause yet.

**Reproduction comment**

https://github.com/codepath/pathreview-ai301-fa26-s3/issues/71#issuecomment-6392546062

# Reproduction Report: Issue #71

**Environment:** macOS 26.2 (arm64), Python 3.14.2, pytest 9.1.1

**Setup:** Used the existing `.venv` (`make setup` on a fresh clone).

**Steps:**
```bash
.venv/bin/pytest tests/unit/test_readme_parser.py -k heading_hierarchy --runxfail -v
```

**Expected:** The test's markdown contains `#`, `##`, `###` headings, so `_extract_heading_hierarchy` returns a non-empty list.

**Actual:** The fixture is indented 8 spaces, so the parser finds zero headings and `assert len(headings) > 0` fails.

**Evidence:**
```text
>       assert len(headings) > 0
E       assert 0 > 0
E        +  where 0 = len([])
tests/unit/test_readme_parser.py:156: AssertionError
```

Without `--runxfail`, the test reports XFAIL.

**Conclusion:** Reproduced. The parser is correct; the fix belongs in the test (dedent the fixture, remove the xfail marker).

[Include any AI-use disclosure required by the repository's policy, exactly as posted.]

## Eval iterations

**Run history**

19/20 → 19/20

**Package analysis**

**Package:** `pkg-20`

**Rubric decision:** Reject

**Gold label:** Reject

**Explanation:** The package contains otherwise strong reproduction evidence, but it does not disclose AI assistance even though the repository's stated policy requires disclosure. The rubric's repository-conventions and AI-disclosure check treats missing required disclosure as a failure, so the package is rejected, matching the gold label.

**Check rationale**

**Exact check from `tools/repro-check/rubric.md`:**

> The package follows applicable repository rules. When the repository requires disclosure of AI assistance, the relevant comments or report explicitly and accurately disclose that assistance. Missing required disclosure, violating an explicit contribution rule, or misrepresenting the work fails this check.

**Rationale:** I made AI disclosure an explicit part of a required check rather than relying on a general instruction to follow repository conventions. This makes missing required disclosure a clear reason to reject a package, even when the technical reproduction evidence is strong.

**Trade-offs**

The change corrected the `pkg-20` disclosure case: the final run rejected it, matching the gold label, and the disclosure category improved to 1/1. The final run still disagreed on `pkg-19`, which the rubric accepted even though the gold label was reject. The change therefore fixed the disclosure gap without eliminating every disagreement elsewhere.
