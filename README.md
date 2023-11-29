# TaskFlowAI - README

## App Specifications v1.0

### Project Overview
TaskFlowAI is a web application designed to integrate a Large Language Model (LLM) with a Notion-based knowledge base. Its aim is to enhance task management, decision-making, and efficiency.

### User Experience
- **Web Interface:** Accessible via any standard web browser.
- **User Interaction Features:**
  - Task Management: Create, modify, and update tasks.
  - Data Input: Enter task-related information via chat interface.
  - Task Summarization: Export weekly task summaries to Notion.
  - Task Categorization: Group tasks for organized viewing.
  - User Draft Interaction: Approve, deny, or edit LLM-generated drafts.
- **Examples of Interactions:**
  - Create high-priority tasks with due dates.
  - Change task status.
  - Generate summaries for specific task types.
  - Update multiple task tags.
  - Approve or modify LLM-generated drafts.

### LLM Capabilities
- Suggest task modifications based on Task Database insights.
- User support through draft modification suggestions and critiques.
- Summary Generation with Notion export functionality.
- Knowledge Base Integration for contextual data access.
- Draft Tracking for enhanced future suggestions.

### Task Parameters
- **Priority:** Urgency level (1 to 100).
- **Status:** Current state (Open, In Progress, Closed).
- **Category:** Task type (e.g., Family, Work).
- **Tags:** Max 5, alphanumeric characters.
- **Due Date:** Format YYYY-MM-DD.
- **Creation Date:** Auto-set, format YYYY-MM-DD.
- **Last Modification:** Auto-update, format YYYY-MM-DD.
- **Week of Work:** Integer between 1-52.
- **Proposed Resolution:** Max 500 characters.
- **Accepted Resolution:** Max 500 characters.
- **Effort Required:** Estimated hours.
- **Automation Capability:** Boolean (Yes or No).

### Features
- Efficient Task Management with categorized parameters.
- Interactive User-LLM Dialogue.
- Automated Summaries exported to Notion.
- Notion Integration for context-aware suggestions.
- CI/CD Workflow for consistent updates.

### Technical Framework
- **GitHub:** Code storage and documentation.
- **Streamlit:** Interactive UI elements.
- **Langchain:** Connects LLM to the application.
- **Notion:** Dynamic knowledge base.
- **OpenAI:** Large Language Model source.
- **Database System:** Task data management.

## Milestones and Tasks for First Release

### Milestone 1: Initial Setup and Framework
- Project initialization, framework selection, environment setup, CI/CD setup, and initial testing setup.

### Milestone 2: Core Application Structure
- Wireframe creation, UI development, database and Notion integration, LLM integration, and application structure testing.

### Milestone 3: Task Management Features
- Task creation module, task categorization, validation rules implementation, and feature testing.

### Milestone 4: User-LLM Interaction
- Draft interaction system, draft tracking, task suggestion system, and interaction testing.

### Milestone 5: Advanced Features and Testing
- Automated summary generation, user support features, advanced and comprehensive testing.

### Milestone 6: Final Review and Deployment
- Final testing and validation, documentation finalization, and deployment.

---
TaskFlowAI – Enhancing Task Management Through AI Integration
