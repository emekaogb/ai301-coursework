# Rubric: is this reproduction package ready to post?

## Checks

| Check | Evidence | Pass condition | Weight |
|---|---|---|---|
| Environment recorded | The repro report's environment record, including relevant software versions, operating system, and configuration | The recorded details are sufficient to understand the conditions under which the reproduction was attempted. Missing details that could materially affect the result fail this check. | required |
| Steps followable | The reproduction steps and the referenced commands, inputs, or setup artifacts | A contributor unfamiliar with the author's session could follow the steps using the provided information without guessing at essential actions or inputs. | required |
| Target behavior demonstrated | The output excerpt, screenshots, logs, or other artifacts read against the issue's description of the expected and actual behavior | The evidence demonstrates the reported behavior or a clearly equivalent manifestation of it. Evidence of an adjacent or unrelated problem does not pass. | required |
| Outcome supported | The reproduction artifacts and results, including any error output or evidence that the issue could not be reproduced | The stated outcome matches the evidence. A cannot-reproduce result passes when the documented attempt provides credible evidence that the issue did not manifest under the recorded conditions. Claiming successful reproduction without supporting evidence fails. | required |
| Repository conventions and AI disclosure | The claim comment and repro report compared with the repository's contribution instructions and AI-use policy | The package follows applicable repository rules. When the repository requires disclosure of AI assistance, the relevant comments or report explicitly and accurately disclose that assistance. Missing required disclosure, violating an explicit contribution rule, or misrepresenting the work fails this check. | required |
| Evidence is easy to verify | The claim comment's references to the report and the report's links or paths to supporting artifacts | A reviewer can locate and inspect the evidence needed to assess the result without relying on unsupported assertions. Minor presentation issues do not fail this check if the evidence remains verifiable. | preferred |

## Verdict rule

Accept if every required check passes. Reject if any required check fails or is unclear. Preferred checks may improve the package but never change the verdict. A cannot-reproduce outcome can pass when the evidence supports it; an unsupported or incorrectly targeted reproduction cannot.

