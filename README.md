# Task Management Integration Application

## Project Overview
This web application integrates a Large Language Model (LLM) with a Notion-based knowledge base to enhance task management. It aims to improve decision-making and task efficiency through advanced user-LLM interactions.

## User Experience
- **Web Interface**: Accessible via standard web browsers.
- **Task Management**: Create, modify, update, and categorize tasks.
- **Data Input**: Enter task-related information through a chat interface.
- **Task Summarization**: Weekly task summaries with Notion export.
- **User Draft Interaction**: Approve, edit, or deny LLM-generated drafts.

## LLM Capabilities
- **Task Interaction**: Suggests task modifications based on database insights.
- **User Support**: Provides draft modification suggestions, proposes efficient follow-up prompts, and recommends task parameters.
- **Summary Generation**: Automated creation of weekly summaries for Notion.
- **Knowledge Base Integration**: Accesses Notion for contextual data.
- **Draft Tracking**: Records user-approved drafts for future reference.

## Task Parameters

| Parameter             | Description                                   | Validation Rules                           |
|-----------------------|-----------------------------------------------|--------------------------------------------|
| Priority              | Indicates the task's urgency level.           | Must be a value from 1 (high priority) to 100 (low priority) |
| Status                | Current state of the task.                    | Values like Open, In Progress, Closed      |
| Category              | Type of task (e.g., Family, Work, Personal growth). | Predefined categories in a dropdown       |
| Tags                  | Keywords for task categorization.             | Max 5 tags; alphanumeric characters        |
| Due Date              | Deadline for task completion.                 | Future date, format YYYY-MM-DD             |
| Creation Date         | Date when the task was created.               | Auto-set; format YYYY-MM-DD                |
| Last Modification     | Date of last task update.                     | Auto-update; format YYYY-MM-DD             |
| Week of Work          | Week number associated with the task.         | Integer between 1-52                       |
| Proposed Resolution   | Suggested solution or closure.                | Text input, max 500 characters             |
| Accepted Resolution   | Resolution agreed upon or implemented.        | Text input, max 500 characters             |
| Effort Required       | Estimated work effort needed.                 | Integer representing hours                 |
| Automation Capability | Task suitability for automation.              | Boolean: Yes or No                         |

## Features
- Task Management
- User-LLM Interaction
- Automated Summaries
- Knowledge Base Integration
- CI/CD Workflow

## Technical Framework
- **GitHub**: Code storage, documentation, version control.
- **Framework**: Django.
- **Streamlit**: User interface.
- **Langchain**: Connects LLM to the application.
- **Notion**: Dynamic knowledge base.
- **OpenAI**: LLM provider.
- **Database System**: MongoDB (for task storage).
- **Vector Database**: Milvus (for the Knowledge repository).
