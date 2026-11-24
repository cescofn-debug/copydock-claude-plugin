---
description: Check the user-facing copy in a file, a folder or your current changes against the house style, and list what to fix.
argument-hint: "[file or folder; leave out to check your uncommitted changes]"
---

Check the user-facing copy in: $ARGUMENTS

If nothing was given, check the copy added or changed in the current changes (`git diff HEAD`, plus untracked files). If there are no changes, say so and ask which file or folder to check.

Follow the copy-dock skill. Then:

1. **Find the copy.** Collect the words people read: text between tags, labels, placeholders, alt text, titles, tooltips, toasts and alerts, thrown error messages, and values in string or translation files. Skip code, keys, class names, URLs, comments, tests and log messages. Note the file and line of each.
2. **Check it.**
   - With Copy Dock connected: call `get_house_style` once, then `check_copy` on each string (pass `copy_kind: "ux"` for product screens). For strings that replace existing approved copy, pass the old text as `shipped_text`.
   - Not connected: review each string against `references/starter-house-style.md` and the guide for its kind of copy, and say that this is a review against general rules, not Copy Dock's code checks.
3. **Report.** Start with one line: how many strings were checked and how many need changes. Then a table of only the strings that need changes: file and line, the current text, what's wrong, and a suggested fix that follows the house style. If everything passes, say so and stop.
4. **Offer to apply the fixes.** Don't edit any file until the person says yes. When applying, change only the text, keep variables, keys and markup intact, and run the check again on the changed strings to show they pass.
