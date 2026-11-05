# Design thinking and methodology

The rationale below follows the implemented notes-to-proposal and transcript-to-proposal workflows and the issues recorded during testing. The focus is on the commercial handoff rather than the private drafting instructions.

## Start with what can go wrong after discovery

A discovery conversation contains problems, possibilities, objections, tentative scope and commercial discussion. Those are not all approved commitments. A polished proposal can hide that distinction if the process moves directly from transcript to presentation.

The design therefore treats the proposal as the result of reviewed information. Drafting is useful, but the salesperson remains responsible for deciding what was established and what can be promised.

## Support two starting points

Some calls already have structured notes; others leave a transcript that still needs interpretation. The manual-notes version allows a salesperson to start from reviewed information. The transcript version adds extraction and an editable review step before proposal generation.

This division avoids making AI extraction mandatory when the salesperson already has accurate notes. It also makes the extra risk of transcript interpretation visible when extraction is used.

## Keep evidence close to the review

An extracted field is easier to assess when the salesperson can see the supporting words and correct the interpretation. Missing or unsupported details should remain unresolved rather than be filled in for the sake of a complete-looking form.

A supporting excerpt is useful evidence, but it is not semantic approval. The words may be present while the model misunderstands whether they describe an existing problem, a suggested solution or an exclusion. Human review is intended to resolve that distinction before it reaches the proposal.

## Separate drafting from commercial authority

Discussing a budget is different from approving a price. Mentioning a desired date is different from committing to a delivery milestone. The process keeps approval-sensitive commercial fields separate from the narrative the model drafts.

This is a deliberate limit on automation. Recording an approval reference does not itself establish that the approver authorised the terms. The salesperson must verify that the entered terms are supported by the relevant decision or agreement.

The presentation remains a draft until it has been reviewed. Automatic sending is outside the verified flow.

## Design for clarity, then test for lost meaning

A consistent presentation structure makes the handoff easier to review. Short slides are useful for a proposal conversation, but summarisation can remove qualifications that matter commercially.

Testing revealed this trade-off: the longer reviewed notes retained a scope exclusion while the shorter slide summary omitted it. This means successful generation and a clean layout are insufficient acceptance criteria. The final review needs to compare the proposal with the notes, particularly for inclusions, exclusions, timing and commercial terms.

The design lesson is to evaluate the promises the document appears to make, not just whether it looks finished.

## Validate different layers of the process

The evidence is considered in layers. Input handling checks whether a file or text can be processed. Extraction checks whether fields have source support. Draft validation checks whether the generated content fits the expected structure. Output review checks the presentation itself. Live integration tests establish that the connected services can complete the path.

None of those alone demonstrates customer acceptance, legal approval or improved win rates.

| Decision | Reason | Trade-off |
|---|---|---|
| Editable review before drafting | Keep the salesperson in control of meaning | Requires deliberate review time |
| Leave missing details unresolved | Avoid confident invention | The salesperson may need another clarification |
| Keep approval-sensitive terms separate | Avoid converting discussion into commitment | The process cannot autonomously complete every proposal |
| Use a consistent presentation structure | Make review and handoff easier | Concise summaries may omit important detail |
| Keep sharing manual | Allow a final commercial check | The workflow does not complete the whole sales follow-up |

## Evidence and next improvements

Retained live integration tests show proposal generation with fictional inputs, including the transcript review path. They also show that an unknown email remained blank and discussed terms were not promoted to approved pricing. These are bounded test outcomes, not real-customer adoption or measured time savings.

Further work should focus on preserving exclusions, checking the meaning of extracted fields and evaluating a wider range of transcripts. The goal is a useful draft whose meaning survives the handoff, with commercial responsibility remaining clear.

[Project status](README.md) · [Conceptual architecture](architecture.md)
