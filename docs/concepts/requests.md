# Requests

**Requests** in Intrigma are user-submitted preferences that affect how the schedule is built. They allow users to communicate their availability, preferences, or unavailability to schedulers during the planning process.

Requests are used primarily to guide automation and inform manual scheduling decisions, but they do not directly place or remove assignments.

---

## Request Types

There are three main types of requests in Intrigma:

1. **Time Off Requests**
   - Indicate that a user prefers not to work on a specific day or shift.
   - Can be hard (unavailable) or soft (preferred).
   - Can be partial-day or full-day requests.
   - Most common for vacation days or known unavailability.

2. **Work Requests**
   - Express interest in working a specific shift or date.
   - Do **not** guarantee assignment but are considered during automation.
   - Useful for part-time or flexible staff indicating preferred work times.

3. **Scheduled Requests** *(if enabled)*
   - Block time for pre-scheduled obligations (e.g., clinic rotations, teaching).
   - Act as placeholders and can potentially be auto-assigned or treated as fixed.
   - May come from external sources or admins.

---

## Request Periods

Requests are submitted **within scheduling periods** that have defined start and deadline dates:

- **Request Start Date** – When users are allowed to start submitting requests.
- **Request Deadline** – Last date requests will be considered.
- Late requests may be denied or ignored based on system configuration.

Schedulers can configure reminders and visibility per period to guide users through request timelines.

---

## Request Statuses

Each request has a **status**:

| Status | Description |
|--------|-------------|
| `Pending` | Submitted but not yet approved |
| `Approved` | Accepted by scheduler (optional for Free Edition) |
| `Denied` | Rejected by scheduler or system rules |
| `Expired` | Submitted after the deadline (optional handling) |
| `Auto-Accepted` | Accepted automatically if no manual review required |

In the Free Edition, requests are typically **auto-accepted**, and approval workflows are minimal.

---

## User Limits & Constraints

Schedulers can define **limits on requests**, including:

- Number of requests per period
- Number of days off in a week or month
- Restrictions by shift type or day of week

These rules help balance fairness and avoid over-requesting.

---

## Automation Considerations

- **Time off requests** are interpreted as *constraints* by the automation engine.
- **Work requests** are interpreted as *preferences*.
- If a user has both availability overrides and requests, **availability takes precedence**.
- Requests do not guarantee assignments — they only influence rule-based decisions.

---

## Reminders and Notifications

Admins can configure automatic **email reminders** to notify users:

- When the request window opens
- As the deadline approaches
- For missing or incomplete requests

Reminder settings are controlled in the **Reminders** module and can be tailored per scheduling period.

---

## Request Swaps

In some versions of Intrigma, users may also submit **Shift Swap Requests** to exchange shifts with another user.

!!! note
    Shift Swaps are optional and may not be enabled in Free Edition.

---

## Related Topics

- [Availability](../features/availability/overview.md)
- [Deadlines & Reminders](../features/requests/deadlines-reminders.md)
- [User Limits](../features/requests/user-limits.md)
- [Request Approval Process](../features/requests/approval-process.md)
- [Request FAQ](../../faq/requests-faq.md)
