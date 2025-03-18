# RFC-0001: GitHub RFC Process

- **RFC Number**: 0001
- **Title**: Establish a Formal GitHub-Based RFC Process
- **Author**: Mark Schmidt
- **Created**: 2025-03-05
- **Status**: Accepted

## Summary

This RFC proposes the formal adoption of a GitHub-based RFC (Request for Comments) process for the Naptha Stack. This process aims to formalize community discussion, improve transparency, document key design decisions, and increase overall collaboration quality on significant changes.

## Motivation

Currently, contributors to the Naptha Stack submit informal RFCs without a standardized structure or repository for organized discussion and archiving. This can lead to fragmented discussions, undocumented decisions, and duplicated efforts. Establishing a formal RFC process will provide clarity, facilitate organized feedback, and better document project evolution.

## Detailed Proposal

### Repository Setup

A dedicated repository named NapthaAI/RFCs will be created.

- Template: A Markdown template (TEMPLATE.md) outlining the RFC structure will be provided.
- Directory Structure: RFCs will reside in the /RFCs repository root with filenames matching a numbering scheme based on the PR number when the RFC is merged (e.g., rfc-001-process.md). Until merged, RFCs should use a descriptive working title (e.g., rfc-github-process.md).
- RFC Lifecycle: RFCs will progress through clearly defined statuses (Draft, Review, Final, Withdrawn).

### RFC Structure

RFCs must include the following sections:
- Metadata: Title, Author(s), Creation Date, PR Number, Status.
- Summary: Briefly describes the proposal.
- Motivation: Clearly states the problem and rationale.
- Detailed Explanation: Technical and high-level details of the proposed solution.
- Rationale and Alternatives: Explains the chosen approach and alternatives considered.
- Impact and Trade-offs: Discusses compatibility, performance, security, and other relevant impacts.
- Unresolved Questions: Lists open questions to be addressed before acceptance.
- References: Links to prior discussions, related RFCs, and external resources.

### Workflow
- Contributors fork the RFC repository, copy the TEMPLATE.md, and draft their RFC.
- Contributors submit an RFC by opening a pull request against the main repository.
- Discussions and feedback occur within the pull request.
- RFC authors iterate based on community feedback, appending new commits without rewriting history.
- When the proposal reaches general consensus, a core Naptha Stack maintainer initiates a 10-day Final Comment Period (FCP).
- After successful FCP, RFCs are merged (accepted), postponed, or rejected (closed with rationale).

### Approval and Decision Making
- RFCs are approved based on rough consensus from the Naptha Stack core maintainers.
- RFCs enter a 10-day Final Comment Period (FCP) before final approval.
- RFCs that are rejected or postponed will be clearly documented.

### Post-Acceptance
- Accepted RFCs are merged into the repository and tracked for implementation.
- A corresponding implementation issue will be opened in the relevant Naptha Stack repository, labeled appropriately (e.g., implementation-tracking).

### Amendments and Updates
- Minor updates to accepted RFCs can be directly made. Major changes require a new RFC.

## Impact and Trade-offs

### Positive Impacts
- Improved documentation of design decisions
- Better organized community discussions
- Clearer process for major changes
- Enhanced transparency in decision-making

### Trade-offs
- Additional overhead in the contribution process
- Potential for over-engineering of small changes
- Need for maintainers to dedicate time to RFC review
- Learning curve for new contributors

### Compatibility
- This process is compatible with existing GitHub workflows
- No technical changes required to existing codebases
- Can be gradually adopted across different Naptha Stack components

### Performance Considerations
- Minimal performance impact as this is a documentation and process change
- May slightly increase time to merge significant changes due to formal review process

### Security Considerations
- Enhanced security through better documentation of security-related changes
- Clearer process for security-critical RFCs

## Drawbacks
- Slight overhead in formalizing the process, which may initially slow contributions.
- Risk of over-engineering discussions for small changes.

## Future Possibilities
- Consider automating parts of the RFC lifecycle with bots or GitHub Actions.
- Expanding sections for specific needs (security considerations, UX impact).

## Unresolved Questions
- Should RFC authors explicitly be responsible for implementing their proposals, or can this responsibility be shared more widely?
- When and how should an RFC be considered "stale"?

## References
- Ethereum Improvement Proposals (EIP): https://github.com/ethereum/EIPs
- Rust RFC Process: https://github.com/rust-lang/rfcs
- Concourse-CI RFC Process: https://github.com/concourse/rfcs

