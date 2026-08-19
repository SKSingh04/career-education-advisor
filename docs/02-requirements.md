# One-Stop Personalized Career & Education Advisor

## 1. Purpose

This document defines the functional and non-functional requirements for the **One-Stop Personalized Career & Education Advisor**.

The requirements establish the expected behavior, capabilities, constraints, and quality standards of the system and will serve as a reference for UI/UX design, frontend development, backend development, database design, recommendation logic, and testing.

The initial requirements focus on the **Minimum Viable Product (MVP)** required to demonstrate the core value of the platform.

---

## 2. MVP Definition

The MVP should provide a complete user journey from collecting a user's profile and preferences to generating personalized career recommendations and providing actionable guidance.

The core MVP journey is:

```text
User Registration / Login
          ↓
User Profile & Onboarding
          ↓
Personal Assessment
          ↓
Career Analysis
          ↓
Career Recommendations
          ↓
Career Details & Suitability Explanation
          ↓
Skill Gap Analysis
          ↓
Personalized Learning Roadmap
          ↓
Relevant Learning Resources
          ↓
Progress & Next Steps
```

The MVP should prioritize **personalization, explainability, and actionable guidance** over advanced features.

---

# 3. Functional Requirements

## 3.1 User Authentication

The system shall provide a mechanism for users to create and access their accounts.

### Requirements

* Users shall be able to register an account.
* Users shall be able to log in to their account.
* Users shall be able to log out.
* The system shall securely handle user authentication information.
* The system shall prevent unauthorized access to user-specific information.
* The system should provide appropriate validation and error messages for invalid authentication attempts.

---

## 3.2 User Onboarding

The system shall collect the information required to generate personalized recommendations.

### Requirements

The onboarding process should collect relevant information such as:

* Educational qualification
* Current academic status
* Field/stream of education
* Existing skills
* Skill proficiency where applicable
* Areas of interest
* Preferred career domains
* Strengths and preferences
* Career goals
* Learning objectives

The system should divide the onboarding process into manageable sections rather than presenting all questions on a single screen.

The system should provide a visible indication of onboarding progress.

Users should be able to review or modify their information before completing onboarding.

---

## 3.3 User Profile

The system shall maintain a user profile containing information relevant to career and education guidance.

### Requirements

The user should be able to:

* View their profile.
* Edit their personal information.
* Update educational information.
* Add or remove skills.
* Update interests and preferences.
* Update career goals.
* Review their assessment information.

Changes to the profile should be reflected in future recommendations where applicable.

---

## 3.4 Personal Assessment

The system shall provide an assessment mechanism to understand the user's interests, preferences, strengths, and career orientation.

### Requirements

* The assessment shall contain structured questions.
* Questions may use formats such as multiple choice, rating scales, or selectable options.
* The system shall record the user's responses.
* The assessment should provide clear progress indicators.
* Users should be able to navigate between assessment sections where appropriate.
* The system should validate required responses before allowing completion.
* Assessment results should contribute to the recommendation process.

The assessment should focus on information that can meaningfully influence career recommendations rather than collecting unnecessary personal information.

---

## 3.5 Career Recommendation

The system shall generate personalized career recommendations using information collected from the user's profile and assessment.

### Requirements

The recommendation system should consider factors such as:

* Education
* Skills
* Skill proficiency
* Interests
* Strengths
* Preferences
* Career goals
* Assessment responses

The system should provide multiple relevant career options rather than presenting only a single career.

Each recommendation should include an indication of suitability, such as:

* Match percentage
* Suitability score
* Match category
* Or another understandable representation

The recommendation system should prioritize explainability.

---

## 3.6 Recommendation Explanation

The system shall explain why a career has been recommended.

For each recommended career, the system should identify relevant positive factors, such as:

```text
Why this career may suit you:
- Strong interest in technology
- Existing programming knowledge
- Analytical aptitude
- Relevant educational background
```

Where possible, the system should also identify factors that require further development.

The recommendation should therefore answer:

> **Why was this career recommended to me?**

The system should avoid presenting recommendations as guaranteed or absolute career decisions.

---

## 3.7 Career Information

The system shall provide detailed information about selected career paths.

Career information may include:

* Career description
* Typical responsibilities
* Required skills
* Recommended educational background
* Relevant technologies or knowledge areas
* Career progression
* Entry-level expectations
* Related career paths

The information should be presented in a clear and understandable format suitable for students.

---

## 3.8 Skill Gap Analysis

The system shall identify gaps between the user's current skills and the skills required for a selected career.

### Requirements

For a selected career, the system should:

1. Identify the skills required for the career.
2. Compare those requirements with the user's existing skills.
3. Identify skills that are already sufficiently developed.
4. Identify skills that require improvement.
5. Prioritize important skill gaps where possible.

Example:

```text
Target Career: Data Scientist

Current Skills
✓ Python
✓ Mathematics
✓ Basic Data Analysis

Skill Gaps
⚠ SQL
⚠ Statistics
⚠ Machine Learning
⚠ Data Visualization
```

The skill-gap analysis should serve as the basis for generating personalized learning guidance.

---

## 3.9 Personalized Learning Guidance

The system shall generate a learning path based on the user's selected career and identified skill gaps.

The learning guidance should:

* Prioritize important skill gaps.
* Organize learning topics in a logical sequence.
* Consider the user's existing knowledge.
* Avoid recommending unnecessary repetition of already-developed skills.
* Provide achievable next steps.

The system should communicate the difference between:

```text
Already Know
      ↓
Need to Improve
      ↓
Need to Learn
      ↓
Ready to Apply
```

---

## 3.10 Learning Resources

The system shall provide relevant educational resources associated with recommended learning topics.

Resources may include:

* Courses
* Tutorials
* Documentation
* Videos
* Articles
* Practice platforms
* Projects
* Other educational material

Each resource should provide sufficient information for the user to understand what it is intended for.

Where external resources are used, the system should provide the appropriate source or destination.

Resource recommendations should be relevant to the user's learning roadmap rather than being a generic collection of links.

---

## 3.11 User Dashboard

The system shall provide a centralized dashboard where users can access their career guidance information.

The dashboard should provide access to:

* User profile summary
* Current career recommendations
* Selected career path
* Skill-gap summary
* Learning roadmap
* Recommended resources
* Progress information
* Suggested next steps

The dashboard should provide a clear overview rather than requiring users to navigate through multiple pages to understand their current status.

---

## 3.12 Progress & Next Steps

The system should allow users to understand their progress toward a selected career path.

Where implemented, users should be able to:

* Mark learning activities as completed.
* View completed and pending learning areas.
* Track skill development.
* View upcoming recommended steps.
* Update their progress.

The system should provide actionable next steps rather than simply displaying information.

---

# 4. Recommendation Requirements

The recommendation mechanism is a core component of the system.

## 4.1 Input Factors

The recommendation mechanism should be capable of using:

```text
Education
Skills
Skill Proficiency
Interests
Strengths
Preferences
Career Goals
Assessment Responses
```

## 4.2 Recommendation Output

The system should generate:

```text
Career
Suitability / Match
Reasons for Recommendation
Required Skills
Skill Gaps
Suggested Learning Path
Relevant Resources
```

## 4.3 Explainability

The recommendation mechanism should provide understandable reasoning behind recommendations.

Users should be able to identify which aspects of their profile contributed to a recommendation.

The system should avoid presenting recommendations as definitive decisions about a user's future.

---

# 5. Functional Requirements Summary

| ID    | Requirement                          | Priority |
| ----- | ------------------------------------ | -------- |
| FR-01 | User registration and login          | High     |
| FR-02 | User onboarding                      | High     |
| FR-03 | User profile management              | High     |
| FR-04 | Personal assessment                  | High     |
| FR-05 | Career recommendations               | Critical |
| FR-06 | Recommendation explanation           | Critical |
| FR-07 | Career information                   | High     |
| FR-08 | Skill-gap analysis                   | Critical |
| FR-09 | Personalized learning guidance       | Critical |
| FR-10 | Learning resource recommendations    | High     |
| FR-11 | User dashboard                       | High     |
| FR-12 | Progress and next steps              | Medium   |
| FR-13 | Profile-based recommendation updates | Medium   |

---

# 6. Non-Functional Requirements

## 6.1 Usability

* The platform should be understandable to users with limited technical knowledge.
* Navigation should be simple and consistent.
* Important information should be visually distinguishable.
* Forms should provide clear instructions and validation feedback.
* The system should minimize unnecessary steps.

---

## 6.2 Responsiveness

The application should provide a usable experience across:

* Desktop computers
* Laptops
* Tablets
* Mobile devices

The interface should adapt to different screen sizes without losing important information or functionality.

---

## 6.3 Performance

* Common pages should load within a reasonable amount of time.
* The system should provide loading indicators for operations that require processing.
* Recommendation generation should provide feedback while processing.
* API responses should be optimized to avoid unnecessary delays.

---

## 6.4 Security

* Authentication credentials must be handled securely.
* Passwords must not be stored in plain text.
* User-specific information must be protected from unauthorized access.
* API endpoints requiring authentication should verify the user's authorization.
* Sensitive configuration values should not be exposed in the source code.

---

## 6.5 Reliability

* The system should handle invalid user input gracefully.
* The system should provide meaningful error messages.
* Failure of external resources or APIs should not crash the entire application.
* User data should be stored consistently.

---

## 6.6 Maintainability

* Frontend and backend code should be organized into logical modules.
* APIs should follow consistent naming and response conventions.
* Database structures should be documented.
* Configuration should be separated from application code.
* The project should follow a consistent Git branching and development workflow.

---

## 6.7 Scalability

The architecture should allow the system to be expanded with additional:

* Career paths
* Skills
* Educational resources
* Recommendation factors
* Users
* External data sources
* Intelligent recommendation methods

The initial implementation should not unnecessarily restrict future expansion.

---

## 6.8 Accessibility

The interface should aim to:

* Use readable typography.
* Maintain sufficient visual contrast.
* Provide clear labels for form controls.
* Avoid relying solely on color to communicate information.
* Support keyboard-friendly interaction where practical.

---

# 7. Data Requirements

The system is expected to maintain structured information related to:

### User Data

* User account
* Education
* Skills
* Interests
* Preferences
* Career goals
* Assessment responses

### Career Data

* Career name
* Description
* Required skills
* Relevant education
* Related careers
* Career progression information

### Skill Data

* Skill name
* Category
* Proficiency level
* Career associations

### Learning Data

* Learning topic
* Learning resource
* Resource type
* Difficulty level
* Associated skill
* Recommended sequence

### Progress Data

* User
* Learning item
* Completion status
* Progress information
* Completion date where applicable

---

# 8. System Constraints

The following constraints should be considered during development:

* The project is being developed within the time constraints of the SIH practice project.
* The MVP should prioritize core functionality over feature quantity.
* Recommendation results should be explainable and demonstrable.
* External data sources may have availability, reliability, or access limitations.
* Advanced machine-learning features should only be introduced if they provide measurable value and can be implemented reliably within the project timeline.
* The system should be designed so that future intelligent features can be added without requiring a complete redesign.

---

# 9. MVP Acceptance Criteria

The MVP will be considered functionally successful when a user can complete the following journey:

```text
1. Create / access an account
        ↓
2. Complete their profile
        ↓
3. Complete the personal assessment
        ↓
4. Receive personalized career recommendations
        ↓
5. Understand why careers were recommended
        ↓
6. Select a career
        ↓
7. View required skills
        ↓
8. Identify personal skill gaps
        ↓
9. Receive a personalized learning path
        ↓
10. Access relevant learning resources
        ↓
11. View the information through a centralized dashboard
```

The MVP should demonstrate that the platform can transform user-specific information into **personalized, explainable, and actionable career guidance**.

---

# 10. Future Requirements

The following capabilities are outside the initial MVP and may be considered in later versions:

* AI-powered conversational career advisor.
* Internship recommendations.
* Job opportunity recommendations.
* Certification recommendations.
* Advanced machine-learning recommendation models.
* Career-path comparison and simulation.
* Integration with external educational platforms.
* Integration with employment platforms.
* Advanced progress analytics.
* Mentor or counselor integration.
* Personalized notifications and reminders.

These features should not compromise completion of the core MVP.

---

# 11. Requirement Prioritization

Requirements should be prioritized using the following categories:

### Critical

Required to demonstrate the primary project concept.

* User profile
* Assessment
* Career recommendation
* Recommendation explanation
* Skill-gap analysis
* Personalized learning guidance

### High

Important for a complete MVP experience.

* Authentication
* Career information
* Learning resources
* Dashboard
* Responsive interface

### Medium

Useful but not essential for the initial demonstration.

* Progress tracking
* Recommendation updates
* Advanced profile customization

### Future

Not required for the initial MVP.

* Conversational AI
* Job/internship recommendations
* Advanced ML
* External platform integrations
* Career simulation

---

## 12. Requirement Traceability

The requirements defined in this document will be used as the foundation for subsequent project documentation:

```text
02-requirements.md
        ↓
03-user-flow.md
        ↓
04-features.md
        ↓
05-system-architecture.md
        ↓
06-database-design.md
        ↓
07-api-documentation.md
        ↓
08-development-plan.md
```

Changes to major requirements should be reflected in the relevant downstream documentation to maintain consistency across the project.
