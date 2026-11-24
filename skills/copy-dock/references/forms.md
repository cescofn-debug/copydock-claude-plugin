# Form labels, hints and validation

Good form copy prevents errors before they happen and fixes them fast when they do.

## Labels

- Short noun phrases in sentence case: "Work email", "Company name". No colons, no "Please enter".
- Always visible. Don't rely on placeholder text as the label; it disappears when people type.
- Mark the exception, not the rule: if most fields are required, label the few optional ones "(optional)".

## Hints (help text)

- Only when people need it: format, why you're asking, or what happens next. "We'll send the invoice here."
- Show requirements before the error, not only after: "At least 8 characters, with one number."

## Placeholders

- An example, not an instruction: "name@company.com", "e.g. Acme app". Never the only label.

## Validation messages

- Say how to fix it, next to the field, in plain words: "Enter an email address like name@company.com".
- Validate when the person leaves the field or submits, not on every keystroke.
- Match the label's words: label "Phone number", error "Enter a phone number with your country code".
- Don't blame or shout: no "Invalid!", no red ALL CAPS.
- For a summary at the top of a long form, link each problem to its field: "2 fields need your attention: Email, Postcode."

## Examples

| Don't | Do |
| --- | --- |
| Label: "Please enter your email:" | Label: "Work email" |
| Error: "Invalid format" | "Enter a date like 31/12/2026" |
| Error: "Field required" | "Enter your company name" |
| Hint: "Password" | "At least 8 characters, with one number" |
