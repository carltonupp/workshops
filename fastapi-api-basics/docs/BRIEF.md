---
note for agent: do not use this file - this is only for the user
---
# Brief: Task Tracker API

Your team has been tracking work in a shared spreadsheet, and it has (predictably) descended into chaos. You have been asked to build a lightweight task tracker that the team can interact with programmatically, so it can eventually be wired into Slack bots, scripts and dashboards.

The application should be a backend web API built with Python and FastAPI, managed with uv. Data must persist across restarts.

## Requirements

The MVP should be able to demonstrate the following use cases:

- Create, update and delete a task
- Tasks have a title, optional description, priority (low, medium, high, critical), due date and status (todo, in_progress, done)
- Group tasks into projects
- List all tasks, or filter them by project and/or status
- Mark a task as done
- Enforce the following rules:
  - A task title is required and no longer than 100 characters
  - A new task cannot have a due date in the past
  - A task that is done cannot be moved back to todo
- BONUS: Assign teammates to tasks, and paginate long task lists
