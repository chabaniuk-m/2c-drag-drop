# Functional Requirements (behavior)

[website demo of this project](https://resplendent-cascaron-bd708b.netlify.app/)

1. Adding tasks
   - Typing text into the input and pressing Enter adds the task to the "To Do" column.
   - Empty or whitespace-only submissions are ignored.

2. Moving tasks
   - Users can move tasks between the three columns via direct manipulation (fast, intuitive interaction).

3. Duplicate prevention
   - Before adding a task, the app checks if an identical task (case-insensitive) already exists in any column.
   - If a duplicate exists, show the notification box with text: "This task is already here in <ColumnName> list" (e.g., "Done").
   - When a duplicate is detected, the input field must keep the entered text so the user can edit it.

4. Removing tasks
   - Tasks may only be removed when they are in the "Done" column.
   - Removal is triggered by a distinct deliberate user action (e.g., a double-activation) so accidental deletion is unlikely.

5. Notifications
   - Notifications are non-blocking, clearly visible, and auto-dismiss after a few seconds.
   - Repeated triggers should not cause visual glitches or stacking of multiple notification boxes.
