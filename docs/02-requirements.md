# Requirements

## Overview

The goal of the MVP is to help families organize weekly meal preparation based on multiple individual diets.

The system should transform individual dietary requirements into a practical weekly plan, helping users decide:

* What each family member will eat.
* What should be prepared in advance.
* How much food should be cooked.
* How meals should be assembled.

The MVP prioritizes operational simplicity and focuses on solving the meal-planning problem before introducing analytics, automation, or AI-powered features.

---

# Functional Requirements

## FR-001 — Family Management

The system must allow users to create and manage family members.

Each family member may include:

* Name.
* Age (optional).
* Dietary restrictions (optional).
* Dietary preferences (optional).

---

## FR-002 — Diet Management

The system must allow users to create and manage diets.

A diet belongs to a single family member.

A diet may be created manually or imported from external sources.

Each diet must support:

* Meals.
* Foods.
* Quantities.
* Meal schedules.
* Optional substitutions.

A diet may remain active for multiple weeks.

---

## FR-003 — Ingredient Management

The system must allow ingredients to be defined and reused across diets and recipes.

An ingredient may include:

* Name.
* Unit of measurement.
* Optional metadata.

Examples:

* Rice.
* Chicken breast.
* Ground beef.
* Eggs.

---

## FR-004 — Recipe Management

The system must allow users to create and manage recipes.

A recipe defines how food is prepared.

Each recipe may include:

* Name.
* Ingredients.
* Preparation steps.
* Optional preparation time.
* Optional yield.

Recipes may be associated with meals generated during weekly planning.

---

## FR-005 — Weekly Meal Plan Generation

The system must generate a weekly meal plan based on the diets of all family members.

The generated plan must:

* Cover all days of the week.
* Include all meals defined in each diet.
* Respect dietary requirements.
* Show what each family member will eat.

Example:

* Monday breakfast.
* Tuesday lunch.
* Wednesday dinner.

---

## FR-006 — Weekly Meal Plan Review

The system must allow users to review a generated meal plan before approving it.

Users may:

* Inspect planned meals.
* Replace meals manually (future enhancement).
* Approve the weekly plan.

Meal preparation may only start after approval.

---

## FR-007 — Cooking Plan Generation

After approval, the system must generate a cooking plan for the week.

The cooking plan must describe:

* What should be prepared in advance.
* Total quantities to prepare.
* Which meals depend on each preparation.
* Which family members consume each preparation.

The cooking plan may distinguish between:

* Food prepared during meal prep sessions.
* Food prepared on demand.

---

## FR-008 — Cooking Instructions

The system must generate step-by-step instructions describing how recipes should be prepared.

Instructions must aggregate ingredient quantities for the entire family and for the selected planning period.

Example:

* Cook 2 kg of chicken breast.
* Prepare 1 kg of rice.
* Roast vegetables.

---

## FR-009 — Meal Assembly Instructions

The system must generate instructions describing how prepared food should be divided among family members.

Example:

**Lunch Box #1**

* Guilherme → 110 g rice + 65 g beans + 120 g chicken.
* Karol → 70 g rice + 50 g beans + 80 g chicken.
* Liz → 50 g rice + 35 g beans + 40 g chicken.

---

## FR-010 — Export

The system must allow users to export generated plans.

Supported formats may include:

* Markdown.
* JSON.

Future versions may support:

* PDF.
* Printable formats.

---

# Non-Functional Requirements

## NFR-001 — Simplicity

The MVP must prioritize simplicity over feature completeness.

Solutions should focus on solving the weekly meal-planning problem with minimal complexity.

---

## NFR-002 — Maintainability

The system must be designed to support future extensions without requiring major rewrites.

Future features may include:

* Shopping lists.
* AI suggestions.
* Habit tracking.
* Analytics.
* Mobile applications.

---

## NFR-003 — AI Independence

The MVP must work without AI capabilities.

AI-powered features are optional enhancements and must not be required for core workflows.

---

## NFR-004 — Responsiveness

The application must support both desktop and tablet usage.

---

## NFR-005 — Documentation

All project documentation must be written in English.

---

## NFR-006 — Privacy

The repository is public.

The project must avoid storing sensitive or personal information in version control.

---

# Constraints

The MVP assumes:

* A single household.
* A limited number of family members.
* Weekly meal preparation.
* Shared meal planning.

Multi-family support is explicitly out of scope.

---

# Out of Scope

The following features are intentionally excluded from the MVP:

* Shopping lists.
* Habit tracking.
* Dashboards and analytics.
* Notifications.
* Calendar integrations.
* Mobile applications.
* Multi-family support.
* AI-generated meal suggestions.
* Nutrition recommendations.
* Meal feedback collection.
* Voice interactions.

---

# Future Enhancements

Future versions of the product may include:

* Smart meal suggestions.
* Recipe transformations.
* Alternative meal options.
* Shopping list generation.
* Habit tracking.
* Meal feedback.
* AI-powered insights.
* Native mobile applications.
* Automation and integrations.

---

# Success Criteria

The MVP will be considered successful if it allows a family to:

1. Create or import their diets.
2. Generate a weekly meal plan.
3. Decide what to cook for the week.
4. Follow the generated cooking instructions.
5. Assemble meals correctly.
6. Organize meal preparation with minimal manual effort.
