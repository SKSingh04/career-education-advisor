# One-Stop Personalized Career & Education Advisor

## 1. Purpose

This document describes the main journey a user follows while using the **One-Stop Personalized Career & Education Advisor**.

The user flow focuses on the MVP and shows how a user moves from creating a profile to receiving career guidance and a personalized learning path.

---

## 2. Main User Flow

```text
Landing Page
      ↓
Login / Sign Up
      ↓
User Onboarding
      ↓
Personal Assessment
      ↓
Career Analysis
      ↓
Career Recommendations
      ↓
Career Details
      ↓
Skill Gap Analysis
      ↓
Personalized Learning Roadmap
      ↓
Learning Resources
      ↓
Dashboard & Progress
```

---

## 3. Detailed User Journey

### Step 1 — Landing Page

The user first arrives at the platform.

The landing page should briefly explain:

* What the platform does.
* How it helps students.
* What the user can expect.
* A clear option to get started.

**Primary action:**

```text
[Get Started]
```

The user is then taken to the login or registration page.

---

### Step 2 — Login / Sign Up

The user can:

* Create a new account.
* Log in to an existing account.

After successful login or registration, the user proceeds to onboarding.

---

### Step 3 — User Onboarding

The system collects basic information needed to understand the user's current situation.

Information may include:

* Educational qualification.
* Current education level.
* Field or stream.
* Existing skills.
* Skill proficiency.
* Areas of interest.
* Career preferences.
* Career goals.

The onboarding process should be divided into simple sections rather than showing all questions at once.

A progress indicator should help the user understand how much of the onboarding process is remaining.

```text
Education
   ↓
Skills
   ↓
Interests
   ↓
Preferences
   ↓
Career Goals
```

After completing onboarding, the user proceeds to the personal assessment.

---

### Step 4 — Personal Assessment

The user answers a series of structured questions designed to understand their:

* Interests.
* Strengths.
* Preferences.
* Career orientation.
* Learning preferences.

Questions may use:

* Multiple-choice questions.
* Rating scales.
* Selectable options.

The system should show assessment progress.

```text
Question 1
    ↓
Question 2
    ↓
Question 3
    ↓
...
    ↓
Assessment Complete
```

After completion, the user's information is sent for analysis.

---

### Step 5 — Career Analysis

The system analyzes the information collected during onboarding and assessment.

The analysis may consider:

```text
Education
Skills
Interests
Strengths
Preferences
Career Goals
Assessment Responses
```

The system then identifies career paths that may be suitable for the user.

A loading or processing screen may be displayed while the analysis is being performed.

---

### Step 6 — Career Recommendations

The system presents multiple career recommendations.

Each recommendation should provide a simple indication of suitability.

Example:

```text
Data Scientist
Match: 82%

Software Developer
Match: 78%

Data Analyst
Match: 74%
```

The user can select a career to learn more about it.

The system should avoid presenting the recommendation as a guaranteed or final career decision.

---

### Step 7 — Career Details

After selecting a career, the user can view more information about that career.

The page may include:

* Career description.
* Required skills.
* Educational requirements.
* Typical responsibilities.
* Relevant technologies.
* Career progression.
* Related careers.

The user can then continue to the skill-gap analysis.

---

### Step 8 — Skill Gap Analysis

The system compares the user's current skills with the skills required for the selected career.

Example:

```text
Target Career: Data Scientist

Your Current Skills
✓ Python
✓ Mathematics
✓ Basic Data Analysis

Skills to Develop
⚠ SQL
⚠ Statistics
⚠ Machine Learning
⚠ Data Visualization
```

This helps the user understand:

> **What do I already know, and what do I need to learn?**

The identified skill gaps become the basis for the personalized learning roadmap.

---

### Step 9 — Personalized Learning Roadmap

The system creates a structured learning path based on the user's skill gaps.

Example:

```text
1. Improve SQL
       ↓
2. Learn Statistics
       ↓
3. Learn Machine Learning
       ↓
4. Practice Data Visualization
       ↓
5. Build Projects
```

The roadmap should take the user's existing knowledge into account.

The goal is to provide a practical sequence rather than simply listing skills.

---

### Step 10 — Learning Resources

The system provides relevant resources for the topics in the learning roadmap.

Resources may include:

* Courses.
* Tutorials.
* Videos.
* Documentation.
* Articles.
* Practice platforms.
* Projects.

Resources should be connected to specific learning goals.

Example:

```text
SQL
├── Beginner Course
├── SQL Practice
└── SQL Project

Machine Learning
├── Fundamentals Course
├── Practice Resources
└── Beginner Project
```

---

### Step 11 — Dashboard & Progress

After completing the initial journey, the user can access a centralized dashboard.

The dashboard may show:

```text
Current Career Goal
        ↓
Career Recommendation
        ↓
Skill Gap
        ↓
Learning Roadmap
        ↓
Completed Learning
        ↓
Next Recommended Step
```

The dashboard should allow the user to quickly understand their current position and what they should do next.

---

## 4. Returning User Flow

A returning user should not have to repeat the entire onboarding and assessment process.

Instead:

```text
Login
  ↓
Dashboard
  ↓
Current Career Path
  ↓
Learning Roadmap
  ↓
Progress
  ↓
Next Steps
```

The user should be able to update their profile or assessment information when necessary.

---

## 5. Alternative User Paths

### User wants to explore another career

```text
Dashboard
    ↓
Explore Careers
    ↓
Select Career
    ↓
Career Details
    ↓
Skill Gap Analysis
    ↓
Learning Roadmap
```

### User changes their career goal

```text
Profile / Dashboard
       ↓
Update Career Goal
       ↓
Re-analyze Profile
       ↓
Updated Recommendations
```

### User wants to update their skills

```text
Profile
   ↓
Update Skills
   ↓
Save Changes
   ↓
Recommendations / Skill Gaps Updated
```

---

## 6. Important User Experience Principles

The user flow should follow these principles:

### Simple

The user should not be overwhelmed with too many questions or options at once.

### Personalized

The system should use the user's information throughout the journey instead of providing generic recommendations.

### Explainable

The user should understand why a career was recommended.

### Actionable

The system should provide clear next steps after giving a recommendation.

### Progressive

Information should be presented step-by-step:

```text
Know Yourself
     ↓
Explore Careers
     ↓
Understand Your Gaps
     ↓
Learn
     ↓
Track Progress
```

---

## 7. Complete MVP Flow

The complete MVP journey can be summarized as:

```text
┌───────────────┐
│ Landing Page  │
└───────┬───────┘
        ↓
┌───────────────┐
│ Login / Signup│
└───────┬───────┘
        ↓
┌───────────────┐
│  Onboarding   │
└───────┬───────┘
        ↓
┌───────────────┐
│  Assessment   │
└───────┬───────┘
        ↓
┌───────────────┐
│ Career Analysis│
└───────┬───────┘
        ↓
┌────────────────────┐
│ Recommendations    │
└─────────┬──────────┘
          ↓
┌────────────────────┐
│  Career Details    │
└─────────┬──────────┘
          ↓
┌────────────────────┐
│  Skill Gap Analysis│
└─────────┬──────────┘
          ↓
┌────────────────────┐
│ Learning Roadmap   │
└─────────┬──────────┘
          ↓
┌────────────────────┐
│ Learning Resources │
└─────────┬──────────┘
          ↓
┌────────────────────┐
│ Dashboard & Progress│
└────────────────────┘
```

This flow represents the **core MVP user journey** and should serve as the foundation for the UI/UX design and subsequent frontend development.
