# User Story Template

A User Story is a short description of a piece of value from the perspective of the person who will use or benefit from it. It is not a technical specification — it is a placeholder for a conversation.

The format below is a starting point. What matters is not the format itself, but the thinking behind it: who needs this, why, and how will we know it is done.

## 📋 Story Structure

### Title
`[Short, descriptive name — visible in the backlog]`

### User Story
> **As a** `[type of user / role]`,
> **I want to** `[action or capability]`,
> **so that** `[benefit or outcome]`.

### Context & Notes
`[Any additional context that helps the team understand the story — business rules, edge cases, dependencies, design references, regulatory requirements, or links to relevant documentation. This section is optional but often essential.]`

### Acceptance Criteria
Acceptance criteria define what "done" looks like for this specific story. They should be written so that anyone on the team can verify them independently.

**Format options:**

**Given / When / Then (behaviour-based):**
- **Given** `[initial context or state]`
- **When** `[action is performed]`
- **Then** `[expected result]`

**Checklist (condition-based):**
- [ ] `[Condition that must be true for the story to be accepted]`
- [ ] `[Another condition]`
- [ ] `[Another condition]`

> Use whichever format makes the criteria clearest for your team. Some stories suit Given/When/Then; others are simpler as a checklist. Mixing both in the same story is fine when it adds clarity.

### Out of Scope
`[What this story explicitly does NOT cover — helps prevent scope creep and sets expectations]`

### Dependencies
`[Any other stories, Features, teams, or systems that this story depends on, or that depend on this story]`

### Definition of Ready checklist
- [ ] Story has a clear title and description
- [ ] Business value is understood by the team
- [ ] Acceptance criteria are defined and verifiable
- [ ] Dependencies are identified
- [ ] Story has been discussed in refinement
- [ ] Team has enough information to estimate

## 📝 Example

### Title
Password reset via email

### User Story
> **As a** registered customer,
> **I want to** reset my password via email,
> **so that** I can regain access to my account if I forget my credentials.

### Context & Notes
This flow must comply with GDPR requirements: the reset link must expire after 30 minutes and must not expose the user's email address in the URL. Design reference: Figma link [#].

### Acceptance Criteria
- **Given** the user is on the login screen and clicks "Forgot password"
- **When** they enter a registered email address and submit
- **Then** they receive an email with a password reset link within 2 minutes

- **Given** the user clicks the reset link
- **When** the link is less than 30 minutes old
- **Then** they are taken to a page where they can set a new password

- **Given** the user clicks an expired reset link (older than 30 minutes)
- **When** they land on the reset page
- **Then** they see an error message explaining the link has expired, with an option to request a new one

- [ ] The reset link works only once — it is invalidated after use
- [ ] The email does not expose the user's current password or any sensitive data
- [ ] The flow works correctly on mobile and desktop

### Out of Scope
- Password strength enforcement (covered in a separate story)
- SMS-based reset (not in scope for this PI)

### Dependencies
- Email service must be configured and available in the test environment

*Template by Marina Rosa Bittencourt · [LinkedIn](https://linkedin.com/in/marinarosabittencourt)*
