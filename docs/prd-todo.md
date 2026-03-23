# Product Requirements Document (PRD) - Todo App Upgrade

## 1. Overview

Upgrade the basic Todo app so users can organize work with due dates, priorities, and date-based filters while keeping the implementation simple and teachable. The MVP must remain frontend-only, use local storage only, and avoid backend or external storage changes.

---

## 2. MVP Scope

- Add an optional `dueDate` field stored in ISO `YYYY-MM-DD` format.
- Add a required `priority` field with allowed values `P1`, `P2`, and `P3`.
- Default `priority` to `P3` when no value is provided.
- Add filters for `All`, `Today`, and `Overdue`.
- Keep completed tasks visible in the `All` filter.
- Hide completed tasks in the `Today` and `Overdue` filters.
- Keep all task storage local to the app with no backend or external storage integration.
- Preserve a simple MVP implementation with no backend changes.
- Validate task data as follows:
- `title` is required.
- `priority` must be one of `P1`, `P2`, or `P3`.
- `dueDate` is optional, and invalid date values should be ignored and treated as absent.

---

## 3. Post-MVP Scope

- Visually highlight overdue tasks so they stand out.
- Display priority using color-coded badges.
- Add task sorting with this order: overdue tasks first, then priority from `P1` to `P3`, then due date ascending, then tasks without a due date last.

---

## 4. Out of Scope

- Notifications
- Recurring tasks
- Multi-user features
- Keyboard navigation enhancements
- Backend persistence or external storage