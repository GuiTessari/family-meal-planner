# Requirements

## Introduction

This document describes the functional and non-functional requirements for Family Meal Planner.

The goal is to define the expected system behavior independently from implementation details or technology choices.

---

# Functional Requirements

## FR-001 — Family Management

The system must allow users to create and manage family members.

Each family member must contain:

- Name
- Avatar or profile picture
- Age
- Notes
- Dietary goals

Examples of dietary goals:

- Weight loss
- Muscle gain
- Healthy eating
- Child nutrition

---

## FR-002 — Dietary Preferences

The system must allow users to configure food preferences for each family member.

Preferences include:

- Foods the person likes
- Foods the person dislikes
- Forbidden foods
- Preferred substitutions

Examples:

- Does not eat fish
- Prefers chicken over beef
- Avoids spicy food

---

## FR-003 — Diet Import

The system must allow users to import diet plans from external documents.

Supported formats:

- PDF

Future versions may support:

- Images
- Spreadsheets

The imported data must be reviewed before being saved.

---

## FR-004 — Diet Management

The system must allow users to:

- Create diets manually
- Edit imported diets
- Remove meals
- Add meals
- Configure meal schedules
- Define food quantities
- Define substitution options

---

## FR-005 — Meal Planning

The system must allow users to create weekly meal plans.

Users must be able to:

- Create plans manually
- Accept suggested plans
- Edit generated plans
- Duplicate previous plans

Each plan must include:

- Meals
- Recipes
- Quantities
- Assigned family members

---

## FR-006 — Weekly History

The system must maintain a complete history of meal plans.

Each historical record must contain:

- Creation date
- Planned meals
- Recipes
- Feedback
- Completion status

---

## FR-007 — Shopping Lists

The system must generate shopping lists based on approved meal plans.

Shopping lists must:

- Aggregate ingredients
- Calculate quantities
- Organize items by category

Example categories:

- Proteins
- Vegetables
- Fruits
- Dairy
- Pantry items

---

## FR-008 — Meal Preparation Workflow

The system must provide a guided workflow for weekly meal preparation.

The workflow includes:

1. Meal plan selection.
2. Shopping list generation.
3. Shopping completion.
4. Cooking phase.
5. Meal assembly.
6. Preparation completion.

---

## FR-009 — Recipe Management

The system must allow users to manage recipes.

Each recipe must contain:

- Ingredients
- Preparation instructions
- Preparation time
- Yield
- Notes

Recipes may be reused across meal plans.

---

## FR-010 — Meal Completion Tracking

The system must allow family members to record whether a meal was completed.

Possible states:

- Completed
- Skipped

Each record must contain:

- Date
- Time
- Family member
- Meal reference

---

## FR-011 — Exception Tracking

The system should allow users to record why a meal plan was not followed.

Examples:

- Ate outside.
- Ordered food.
- Forgot the meal.
- Attended an event.

The system may also store replacement meals.

---

## FR-012 — Meal Feedback

The system must allow users to provide feedback about meals.

Supported feedback types:

- Rating
- Text comments

Future versions may support:

- Voice notes

Feedback must remain associated with:

- Recipes
- Meal plans
- Family members

---

## FR-013 — Habit Tracking

The system must provide metrics related to eating habits.

Examples:

- Number of completed meals.
- Weekly consistency.
- Consecutive days.
- Completion percentage.

---

## FR-014 — Dashboard

The system must provide dashboards containing historical and behavioral information.

Examples:

- Meal completion rate.
- Favorite recipes.
- Most skipped meals.
- Weekly performance.
- Historical trends.

---

## FR-015 — AI-Assisted Features

The system may provide intelligent assistance features.

Examples:

- Diet interpretation.
- Meal suggestions.
- Feedback analysis.
- Recipe recommendations.

The absence of these features must not prevent the system from functioning.

---

# Non-Functional Requirements

## NFR-001 — Usability

The application must be simple enough to be used by non-technical users.

The kitchen tablet experience should require minimal interactions.

---

## NFR-002 — Responsiveness

The interface must work on:

- Desktop browsers
- Tablets
- Mobile devices

---

## NFR-003 — Reliability

User data must persist across sessions.

The system must avoid data loss.

---

## NFR-004 — Extensibility

The architecture should allow future support for:

- Multiple families
- Native applications
- Calendar integrations
- Grocery integrations

---

## NFR-005 — Maintainability

The system should be organized in a way that facilitates long-term maintenance and future enhancements.

---

## NFR-006 — Privacy

Personal information and dietary data must remain private.

The system must avoid exposing sensitive information.

---

## NFR-007 — Offline Tolerance

Temporary connection failures should not compromise core user workflows.

---

# Constraints

Initial constraints:

- Single-family support.
- Household usage.
- Kitchen tablet as the primary device.
- Manual workflows must work without AI assistance.
