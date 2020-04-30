# Scheduler - Recurrence improvements

# The Problem

The Scheduler component has lot of problems with a complex recurrence rules ([iCalendar RFC2445](https://tools.ietf.org/html/rfc2445)):

For example if start month: `May` and recurrence rule: `FREQ=MONTHLY;BYDAY=FR;BYMONTHDAY=22,23,24,25,26,27,28;INTERVAL=2` then component will generate:
	`May`, `August`, `November` and so on (every 3 months)

Instead of expected:
	`May`, `Jul`, `Sep` and so on (every 2 months)

# The Proposed Solution

We plan to:

- replace our recurrent appointments generator with [RRule](https://github.com/jakubroztocil/rrule) library,
- improve our recurrent editor to edit more complex recurrent rules.

# Installation

Follow the installation guide from the [release page]([https://github.com/DevExpress/DevExtreme/releases](https://github.com/DevExpress/DevExtreme/releases)) and leave us feedback on this topic.

# We Need Your Feedback

## Take a Quick Poll

Do you find improvements in recurrence useful?

- No, I do not need them
- Yes, and the proposed implementation meets all my requirements
- Yes, but the proposed implementation does not meet my requirements (Please provide more details in the GitHub comments or via the Support Center)
- Other: // (user answer)

# Get Notified of Updates

Subscribe to this thread or to our [Facebook]([https://www.facebook.com/DevExpress.DevExtreme/](https://www.facebook.com/DevExpress.DevExtreme/)) and [Twitter]([https://twitter.com/devextreme](https://twitter.com/devextreme)) accounts for updates on this topic.
