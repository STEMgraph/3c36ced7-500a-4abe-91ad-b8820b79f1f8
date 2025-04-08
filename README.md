<!---
{
  "depends_on": [],
  "author": "Stephan Bökelmann",
  "first_used": "2025-04-08",
  "keywords": ["scrum", "acceptance criteria", "user story", "project management"]
}
--->

# Writing Effective Acceptance Criteria

## Introduction
Acceptance criteria are the foundation of a shared understanding between developers, designers, and stakeholders. They help define when a User Story is “done” and guide both implementation and testing. Clear, actionable criteria reduce ambiguity, enable test automation, and improve product quality.

For example, take the following User Story:
> *As a user, I want to reset my password so that I can access my account if I forget it.*

Weak acceptance criteria might say:
- "User can reset password."

This is vague and not testable. A better set of criteria could be:
- ✓ A reset email is sent to the registered email address.
- ✓ The reset link expires after 1 hour.
- ✓ The new password must meet complexity requirements.

Or, using the Gherkin format:
```
Given I have requested a password reset
When I click the link in the email
Then I am able to set a new password that meets security rules
```

Such criteria not only guide developers but also help QA teams write tests and stakeholders understand what “done” really means. In this exercise, you will practice writing and evaluating acceptance criteria using real-world examples. of a shared understanding between developers, designers, and stakeholders. They help define when a User Story is “done” and guide both implementation and testing. Clear, actionable criteria reduce ambiguity, enable test automation, and improve product quality. In this exercise, you will practice writing and evaluating acceptance criteria using real-world examples.

## Further Readings
- Dan North: [Introducing BDD](https://dannorth.net/introducing-bdd/)
- Agile Alliance: [Acceptance Criteria](https://www.agilealliance.org/glossary/acceptance-criteria)
- Cucumber: [Gherkin Syntax](https://cucumber.io/docs/gherkin/)

## Tasks
1. Choose one of the following User Stories or create your own:
   - *As a user, I want to reset my password so that I can access my account if I forget it.*
   - *As a project manager, I want to assign tasks to team members so that responsibilities are clear.*
   - *As a customer, I want to track my order status so that I know when to expect delivery.*

2. Write at least 3 acceptance criteria for the chosen story. Use either:
   - **Checklist format** (✓ The reset link expires after 1 hour)
   - **Gherkin format**:
     ```
     Given I am on the login page
     When I click "Forgot Password" and enter my email
     Then I receive an email with a reset link
     ```

3. Exchange your story and criteria with a peer and:
   - Validate if the criteria are testable, unambiguous, and complete
   - Suggest at least one improvement

## Questions
- What is the difference between acceptance criteria and tests?
- Can a story be implemented without acceptance criteria?
- Who should define the acceptance criteria in a project team?
- How can unclear acceptance criteria lead to defects?

## Advice
Write acceptance criteria collaboratively—ideally during backlog refinement. Keep them simple, specific, and user-centered. Use concrete examples and avoid vague terms like “fast” or “intuitive.” When in doubt, test your criteria by turning them into unit or end-to-end tests.

