# Evidence guide: where proof lives in a reproduction package

## Environment

**Where it lives:** In an eval bundle, inspect the repro report's environment record and compare it with the issue context and repo-facts block. In live mode, inspect the student's draft report and compare the recorded environment with the issue description and repository documentation.

**What good looks like:** The report identifies the relevant operating system, software versions, configuration, and prerequisites needed to interpret the result. Versions or settings that differ from the issue's stated target are explicitly identified rather than presented as equivalent.

## Steps

**Where it lives:** In an eval bundle, inspect the repro report's reproduction steps and any referenced commands, inputs, setup instructions, or artifacts. In live mode, inspect the draft report and verify that its instructions are consistent with the issue and repository documentation.

**What good looks like:** The steps establish the starting state, provide the necessary setup, and explain how to trigger the behavior. A stranger can follow them without guessing at essential commands, inputs, or omitted actions.

## Behavior shown

**Where it lives:** In an eval bundle, inspect the output excerpts, logs, screenshots, test results, and other artifacts alongside the issue context's description of the reported behavior. In live mode, inspect the artifacts linked or included in the draft report and compare them with the behavior described in the GitHub issue.

**What good looks like:** The evidence shows the specific behavior the issue describes, or a clearly equivalent manifestation of it. An error or screenshot that only demonstrates a related feature or unrelated failure does not establish reproduction of the target issue.

## Honesty

**Where it lives:** In an eval bundle, compare the outcome stated in the repro report and claim comment with the environment record, steps, and supporting artifacts. In live mode, compare the student's draft claim and report with the actual evidence they provide.

**What good looks like:** The stated outcome accurately reflects what happened during the documented attempt. A cannot-reproduce result is acceptable when the report provides credible evidence of the attempt and its result; claiming success without supporting artifacts, or presenting an unrelated failure as the target issue, is not.

## Comms

**Where it lives:** In an eval bundle, inspect the claim comment, repro report, issue context, repo-facts block, and any supplied contribution-policy or template information. In live mode, compare the draft claim and report with the issue thread, repository contribution instructions, reporting templates, and applicable AI-use disclosure requirements.

**What good looks like:** The claim comment accurately describes the intended reproduction and does not claim results before evidence exists. The report communicates concrete findings, follows applicable repository rules—including required AI-use disclosures—and avoids boilerplate or unsupported assertions that obscure what was actually observed.

