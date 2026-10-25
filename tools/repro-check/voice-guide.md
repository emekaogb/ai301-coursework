# Voice guide: how I talk upstream

## Who I am in threads

I am an early-career software developer contributing to Path Review and learning the repository's conventions as I go. I aim to communicate what I observed, what I tried, and what I plan to do next without overstating my experience or results.

## Rules I write by

### Rule: Separate plans from completed work

I never describe something as reproduced, fixed, or verified until I have evidence that it happened.

- Wrong: "I've reproduced the bug and will submit the fix soon."
- Right: "I'll work on reproducing the reported behavior and share the results here."

### Rule: Give concrete updates

I name the behavior, command, or result instead of saying I am investigating without explaining what that means.

- Wrong: "I'm looking into this issue and will update everyone."
- Right: "I'll test the README heading parser with the indented fixture and report whether it produces the expected headings."

### Rule: Be honest about uncertainty

I distinguish what the evidence shows from what I suspect, and I say when I cannot confirm a cause or result.

- Wrong: "This is definitely caused by the parser's indentation handling."
- Right: "The issue suggests indentation may be preventing the fixture from producing headings; I'll verify that against the parser's behavior."

### Rule: Keep claims specific to the issue

I connect my comments to the reported behavior and avoid claiming that a broader problem is solved when I have only tested one case.

- Wrong: "This fixes heading parsing across the project."
- Right: "This test checks whether the indented fixture is parsed as containing headings."

### Rule: Respect repository guidance

I check contribution instructions and follow any required format or AI-use disclosure instead of assuming my usual workflow applies.

- Wrong: "The reproduction is ready; I'll post it now."
- Right: "I'll check the repository's contribution requirements and verify the reproduction evidence before posting."

## Things I never post

- Claims that I reproduced, fixed, or tested something when I have not.
- Promises that a fix or review will be completed by a deadline I cannot guarantee.
- Statements that present a guess as a confirmed cause.
- Broad claims of success based on one narrow test.
- Generic status updates that do not explain what I tried or what I will do next.
- Comments that ignore repository contribution rules or required AI-use disclosures.