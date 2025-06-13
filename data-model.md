## 📊 Request Log Schema

| Field Name          | Type       | Description                                                  |
|---------------------|------------|--------------------------------------------------------------|
| Request ID          | String     | Unique ID for each request (e.g., GUID or timestamp)         |
| Submission Date     | DateTime   | When the request was received                                |
| Request Text        | Text       | Full message submitted by the user                           |
| Category            | Text       | Classified type (HR, IT, etc.)                               |
| Confidence Level    | Text       | "High", "Medium", or "Low" – from AI output                  |
| Routing Destination | Text       | Email, Teams channel, or team name the request was sent to   |
| AI Explanation      | Text       | One-sentence rationale from the model                        |
| Status              | Text       | Pending, Routed, Escalated, Closed                           |
| Notes               | Text       | Optional manual annotations or troubleshooting info          |

