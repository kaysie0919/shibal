### Table 5: JOB_PERFORMANCE

| FIELD NAME | DESCRIPTION                          | DATA TYPE | LENGTH | SAMPLE        |
|------------|--------------------------------------|-----------|--------|---------------|
| PERFORMANCE_ID  | Primary key, unique identifier for each performance record.  | Int  | 255  |  HWAKJD8900  |
| JOB_ID  |  Foreign key to the Job_Posting table.  | Int  | 255 | WHEJKA2434  |
| APPLICATION_COUNT  | Number of applications submitted for the job posting.  | Int  | 255  | 4 Applicants Pending  |
| VIEWS_COUNT  | Number of times the job post was viewed by candidates.  | Int  | 255  | 4 Views  |
| OPEN_DATE  | Date when the job posting became active.  | Datetime  |    | 2024-10-05 07:24:00 PM |
| CLOSE_DATE  | Date when the job posting was closed or filled.  | Datetime  |    |  2024-10-05 07:27:00 PM  |
| TIME_TO_FILL  |  Number of days the job post remained open before being filled.  | Int  | 255  |  4 days  |
| UPDATED_AT  |  Date when this performance record was last updated.  | Datetime  |    |  2024-10-05 07:32:00 PM  |

### Table 6: JOB_INTERACTION

| FIELD NAME | DESCRIPTION                          | DATA TYPE | LENGTH | SAMPLE        |
|------------|--------------------------------------|-----------|--------|---------------|
| INTERACTION_ID  | Primary key, a unique identifier for each interaction record.  | Int  | 255  | WJEHWK2414  |
| USER_ID  | Foreign key to the User table (tracks which user interacted).  | Int  | 255  | EKJRNER3432  |
| JOB_ID  | Foreign key to the Job_Posting table (which job was interacted with).  | Int  | 255  | KHEKTHE7544  |
| INTERACTION_TYPE  | Type of interaction (VIEW, APPLY).  | Enum  |    | View  |
| INTERACTION_DATE  | Date and time when the interaction occurred.  | Datetime  |    | 2024-10-05 07:42:00 PM    |
| IS_APPLIED  | Flag to check if the user has applied to the job.  | Boolean  | Applied    |
