# Confirmation dialogs and destructive actions

Ask for confirmation only when an action is hard to undo. Then make the consequence impossible to miss.

## Structure

- **Title as a question naming the action and the object:** "Delete Website redesign?"
- **Body: what will happen, and whether it can be undone.** "This deletes the project and its 42 strings for everyone. You can't undo this."
- **Buttons: the action as a verb, and Cancel.** "Delete project" / "Cancel". The destructive button is styled as destructive; the safe one has focus.

## Rules

- Name the specific thing (its name, the count), not "this item".
- Say who it affects ("for everyone in your workspace") and what's kept ("Your exports stay in Downloads").
- Never "Are you sure?" on its own, and never Yes/No buttons.
- If it can be undone, say how long and where: "You can restore it from Trash for 30 days." Often that means you don't need a dialog at all; an undo toast is better.
- For the most serious actions, ask people to type the name to confirm, and say so plainly.

## Examples

| Don't | Do |
| --- | --- |
| Are you sure? [Yes] [No] | **Delete Website redesign?** This deletes the project and its 42 strings for everyone. You can't undo this. [Delete project] [Cancel] |
| Remove user? [OK] | **Remove Ana from Acme Studio?** Ana loses access straight away. Their drafts stay in the workspace. [Remove Ana] [Cancel] |
| Discard? | **Leave without saving?** Your changes to this string will be lost. [Leave without saving] [Keep editing] |
