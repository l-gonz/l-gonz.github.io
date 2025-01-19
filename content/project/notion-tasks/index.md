---
title: Notion recurring tasks
summary: A system to automate recurring tasks in Notion using Slack, AWS Lambda, and the Notion API.
tags: ["cloud", "api", "python"]
date: 2024-08-28
github: "https://github.com/l-gonz/notion"
links:
  - icon: github
    icon_pack: fab
    name: Repository
    url: https://github.com/l-gonz/notion
---

## About This Project
Notion doesn't include support for recurring tasks in a way that truly mimicks tradional task managers. The only automation that can be triggered when the task database updates (i.e. marking a task as complete) is a notification message published to Slack. To solve this, I built a system that automates updating task due dates using Slack webhooks, AWS Lambda functions, and the Notion API. By integrating these tools, the system detects changes in the Notion Tasks database, processes the updates, and reschedules tasks with the next due date automatically.

UPDATE: Notion has sinced expanded its automations functionality and made this project unnecessary. However, it was still an interesting weekend project.

---

## Key Features
- **Automatic Due Date Updates**: Tasks in Notion are automatically updated to their next due date upon completion.
- **Slack Integration**: Slack acts as a bridge, detecting task updates and triggering AWS Lambda functions.
- **Serverless Architecture**: AWS Lambda and API Gateway ensure efficient and cost-effective operation.
- **Notion API Integration**: Communicates directly with Notion databases to retrieve and update task properties.

---

## Tech Stack
- **Backend**: AWS Lambda (Python), API Gateway
- **APIs**: Notion API, Slack API
- **Workflow Automation**: Slack Webhooks
- **Python libraries**: `notion-client`, `requests`

---

## How I Built It
### System Workflow
1. **Slack to AWS Lambda**:
   - Notion monitors changes to the Tasks database and posts messages to a dedicated Slack channel.
   - Webhooks are triggered by new Slack messages, sending the payload to an AWS Lambda function.

2. **AWS Lambda Function**:
   - Validates the Slack message and extracts task details.
   - Connects to the Notion API using the task's unique ID to retrieve the current task properties.
   - Updates the task's "Due" date to the next scheduled date and resets the "Done" status.

3. **Notion API**:
   - Retrieves and updates task properties, ensuring the database remains accurate and consistent.

### Key Challenges
- **Data Parsing**: Extracting database and task IDs from Slack messages required robust text parsing.
- **Secure Communication**: Ensured secure authentication with Slack and Notion tokens.
- **Real-Time Updates**: Maintained low latency for task updates to feel instantaneous.

![Workflow Diagram](images/notion-tasks/aws.png "Workflow diagram in AWS")

Explore more:
- [GitHub Repository](https://github.com/l-gonz/notion)

---

This project shows how automation can save time and streamline workflows by connecting powerful APIs and cloud services. It’s a practical solution for anyone looking to supercharge their productivity tools.
