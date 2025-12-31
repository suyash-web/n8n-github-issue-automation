# GitHub Issue → Notion Tracker → Slack Alert (n8n Workflow)

## Overview
This n8n workflow automates GitHub issue tracking by listening for newly created issues,
extracting relevant metadata, persisting the data in a Notion database, and notifying
the team via Slack in real time.

The workflow demonstrates event-driven automation, data normalization, and
multi-service integration using n8n.

## Trigger
- GitHub Trigger: Issues → Opened

## Workflow Steps
1. GitHub Trigger listens for newly created issues in a repository
2. Set node extracts and normalizes issue metadata
3. Notion node creates a database entry for tracking
4. Slack node sends a formatted notification message

## Example Slack Notification
:new: New GitHub Issue Created  
• Title: n8n test  
• Author: suyash-web  
• Link: https://www.notion.so/n8n-test-2da52f6ada078125afc2cd13100e12d6  
• Created At: 2025-12-30T23:56:00.000-05:00  
• Status: open

## Tools & Services
- GitHub (issue events)
- Notion (issue tracking database)
- Slack (team notifications)
- n8n Cloud (workflow orchestration)

## Setup Instructions
1. Import the provided JSON workflow into n8n
2. Configure GitHub credentials (Personal Access Token)
3. Configure Notion credentials (Internal Integration Token)
4. Share the Notion database with the integration
5. Configure Slack credentials using a Bot token (xoxb-)
6. Invite the bot to the target Slack channel
7. Activate the workflow
8. Create a GitHub issue to test

## Use Case
Useful for engineering teams that want automatic visibility into new GitHub issues,
centralized tracking, and faster response times without manual updates.

## Notes
- Slack integration uses a scoped bot token for secure message delivery
- Workflow is modular and easily extensible (email, Jira, databases, etc.)
