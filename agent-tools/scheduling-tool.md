Use this tool to manage appointments in Google Calendar on behalf of the client. It supports creating, rescheduling, and cancelling events. The tool receives natural language queries and does **not** interact directly with the client. It checks availability and responds with a success message, an error, or alternative time suggestions based on allowed scheduling rules.

This tool should be invoked only when the user expresses a clear scheduling intent.

## Inputs

- `client_name` (string): The full name of the client.
- `query` (string): A natural language instruction describing the scheduling request.

---

## Query Examples

### Schedule Appointment

- `Schedule a haircut for Tuesday, June 17 at 4:00 PM`
- `Book a consultation on Thursday at 10 AM`

### Reschedule Appointment

- `Reschedule my appointment to Wednesday, June 18 at 3:00 PM`
- `Move my appointment to Friday morning`

### Cancel Appointment

- `Cancel my appointment on June 17`
- `I need to cancel my haircut booking`
