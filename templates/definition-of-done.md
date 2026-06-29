## Definition of Done (DoD)

A Definition of Done establishes the criteria that must be met for a Feature to be considered complete. It is a shared quality standard - agreed by the team, visible to everyone, and applied consistently.

The DoD is not a checklist of tasks. It is the team's commitment to what "done" actually means - so that work is not declared complete when it is only partially finished, and so that quality does not erode sprint by sprint.

**Note on scope:** This DoD operates at the Feature level. A Feature is only considered Done when all its PBIs are complete and the Feature as a whole meets these criteria. Individual PBIs have their own acceptance criteria, which must be met before the PBI can be considered done at story level.

### ✅ Definition of Done - Feature Level ###

A Feature is considered **Done** when:

#### Delivery 
- [ ] All PBIs within the Feature are complete and their acceptance criteria have been verified.
- [ ] The Feature behaves as described in the original scope - and no known gaps between what was agreed and what was built.
- [ ] All in-scope edge cases and error states have been handled.

#### Quality
- [ ] The work has been reviewed (code review, design review, or equivalent depending on the type of work).
- [ ] Testing has been completed at the appropriate level (unit, integration, end-to-end, UAT - as defined by the team).
- [ ] No critical or high-severity defects remain open.
- [ ] Accessibility and performance requirements have been considered where applicable.

#### Documentation & Visibility
- [ ] Relevant documentation has been updated (technical documentation, process documentation, API specs, or equivalent).
- [ ] The work is visible in the team's tracking tool (e.g. Azure DevOps, Jira) with status updated accordingly.
- [ ] The Product Owner has reviewed and accepted the Feature.

#### Integration & Dependencies
- [ ] The Feature works correctly in integration with dependent systems or other Features.
- [ ] No regressions have been introduced in existing functionality.
- [ ] Cross-team dependencies that were unblocked by this Feature have been communicated to the relevant teams.

#### Compliance (where applicable)
- [ ] Regulatory or security requirements relevant to this Feature have been addressed (e.g. GDPR consent flows, PSD2 compliance, audit logging).
- [ ] Data privacy considerations have been reviewed where personal data is involved.

### 📝 How to adapt this for your team

1. **The DoD should reflect your team's actual quality bar.** Not an aspirational one that nobody can reach, and not a minimal one that lets half-finished work through.
2. **Make it visible.** Pin it to the team's board, add it to Confluence (or other documentation platform), put it in the sprint planning template. A DoD that lives only in a document nobody opens does not exist.
3. **Apply it consistently.** The DoD applies to every Feature, every sprint. If the team is regularly unable to meet it, that is a signal, either the DoD needs adjustment, or the team needs support.
4. **Separate DoD from acceptance criteria.** Acceptance criteria are specific to a PBI ("the user can reset their password via email"). The DoD is the quality standard that applies to everything ("no critical defects remain open"). Both matter; neither replaces the other.
5. **Revisit it as the team matures.** A team's Definition of Done should become more demanding over time, not less.

*Template by Marina Rosa Bittencourt · [LinkedIn](https://linkedin.com/in/marinarosabittencourt)*
