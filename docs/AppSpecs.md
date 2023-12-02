# **App Specifications v1.0**

# Project Overview

A web application designed to enhance task management through an integration of Large Language Model (LLM) and a Notion-based knowledge base, focusing on improving decision-making and task efficiency.

## **User Experience**

- **Web Interface:** Accessible via any standard web browser.
- **User Interaction:**
    - **Task Management:** Create, modify, and update tasks.
    - **Data Input:** Enter task-related information via chat.
    - **Task Summarization:** Generate and export weekly task summaries to Notion.
    - **Task Categorization:** Group tasks (e.g., work-related) for organized viewing.
    - **User Draft Interaction:** Approve, deny, or edit LLM-generated drafts.
- **Examples of Interactions:**
    - Creating a high-priority task with a specific due date.
    - Changing task status.
    - Generating summaries for specific task types.
    - Updating multiple task tags simultaneously.
    - Approval: Users approve, deny, or manually edit drafts created by the LLM.

## **LLM Capabilities**

- **Task Interaction:** Suggest task modifications based on Task Database insights.
- **User Support:**
    - Drafts modification suggestions and critiques.
    - Proposes efficient follow-up prompts.
    - Recommends task parameters and knowledge base additions.
- **Summary Generation:** Creates summaries for upcoming weeks, with Notion export functionality.
- **Knowledge Base Integration:** Accesses Notion for contextual data (read-only without user approval).
- **Draft Tracking:** Maintains a record of user-approved drafts for enhanced future suggestions.

## Tasks Parameters:

| Parameter | Description | Validation Rules |
| --- | --- | --- |
| Priority | Indicates the task's urgency level. | Must be a value from 1 (high priority) to 100 (low priority) |
| Status | Current state of the task. | Values like Open, In Progress, Closed |
| Category | Type of task (e.g., Family, Work, Personal groth). | Predefined categories in a dropdown |
| Tags | Keywords for task categorization. | Max 5 tags; alphanumeric characters |
| Due Date | Deadline for task completion. | Future date, format YYYY-MM-DD |
| Creation Date | Date when the task was created. | Auto-set; format YYYY-MM-DD |
| Last Modification | Date of last task update. | Auto-update; format YYYY-MM-DD |
| Week of Work | Week number associated with the task. | Integer between 1-52 |
| Proposed Resolution | Suggested solution or closure. | Text input, max 500 characters |
| Accepted Resolution | Resolution agreed upon or implemented. | Text input, max 500 characters |
| Effort Required | Estimated work effort needed. | Integer representing hours |
| Automation Capability | Task suitability for automation. | Boolean: Yes or No |

# Features

- **Task Management:** Efficient handling of tasks with categorized parameters.
- **User-LLM Interaction:** Interactive dialogue with LLM for task insights and suggestions.
- **Automated Summaries:** Generation and export of task summaries to Notion.
- **Knowledge Base Integration:** Seamless integration with Notion for context-aware suggestions.
- **CI/CD Workflow:** Continuous Integration and Deployment for consistent application updates.

## **Technical Framework**

- **GitHub:** For code storage, documentation, and version control.
- **Streamlit:** Powers interactive user interface elements.
- **Langchain:** Connects LLM to the application.
- **Notion:** Acts as a dynamic knowledge base.
- **OpenAI:** Source of the Large Language Model.
- **Database System:** Manages and organizes task data.