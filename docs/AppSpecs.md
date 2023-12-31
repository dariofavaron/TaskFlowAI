# **App Specifications**

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

## **Terminology**

### **Draft**

- **Definition:**
    - A **draft** is an output generated by the Large Language Model (LLM) in response to user interactions. It represents a preliminary version of content, encompassing modifications, suggestions, or new creations by the LLM.
- **Characteristics:**
    - **Content Range:** Can vary from a single word to a longer document, designed for single-screen viewing.
    - **Visual Distinction:** New or altered content is visually differentiated (e.g., through highlighting or formatting) to distinguish it from existing text.
    - **Editable:** Drafts are designed for user review and editing, allowing approval, modification, or rejection.
    - **User Control:** Each draft requires user interaction—approval (green tick), denial (red X), or editing.
- **Approval Process:**
    - **Individual Modifications:** Each modification in larger documents can be individually accepted or rejected.
    - **Group Approval/Denial:** Users can accept or deny all modifications in a section or the entire document.
    - **Interactive Buttons:** Approvals and denials are facilitated through interactive buttons alongside the draft.
- **Examples:**
    - **New Task Creation:** A draft for a new task includes all relevant details, with new elements highlighted for user review and action.
    - **Status Modification:** Changes in task status are highlighted, enabling easy user management.
    - **Review System:** Features like underlining or format changes emphasize LLM changes, with each being individually manageable.
- **Real-World Example:**
    - **Task Status Change:** Consider a task titled "Water the Plants." Initially, its status is "Backlogged." When the status changes to "Scheduled," the draft reflects this change:
        - Original: "Water the Plants - Status: ~~Backlogged~~"
        - Draft: "Water the Plants - Status: **Scheduled**"
        - In this draft, "Scheduled" is bolded to indicate the new status, while "Backlogged" is struck through, signifying its removal.

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
| Higher Dependance | higher cathegory connected, directly dependent | Already existing cathegory |

# Features

- **Task Management:** Efficient handling of tasks with categorized parameters.
- **User-LLM Interaction:** Interactive dialogue with LLM for task insights and suggestions.
- **Automated Summaries:** Generation and export of task summaries to Notion.
- **Knowledge Base Integration:** Seamless integration with Notion for context-aware suggestions.
- **CI/CD Workflow:** Continuous Integration and Deployment for consistent application updates.

## **Technical Framework**

- **Framework**: Django.
- **GitHub:** For code storage, documentation, and version control.
- **Streamlit:** UI, Powers interactive user interface elements.
- **Langchain:** Connects LLM to the application.
- **Notion:** Acts as a dynamic knowledge base.
- **OpenAI:** Source of the Large Language Model.
- **Database System**: MongoDB, for task storage and knowledge.
- **Virtual Development Environment**: GitHub Codespaces, chosen for its simplicity and integration with GitHub, aligning with our current development needs and future plans for Docker containerization.
- **Deployment**: Docker package

## Future Features

- **Vector Database**: Milvus (for similarity-based retrieval on the Knowledge repositories).