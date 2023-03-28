# GitHub-Jira Integration

Seamlessly integrate GitHub with Jira using GitHub Actions for better project management and collaboration.

## Features

- **Issue Synchronization**: Automatically create a Jira issue when a new GitHub issue is created.
    - Convert GitHub markdown to Jira markup for consistent formatting.
    - Append a reference to the GitHub issue within the Jira issue.
    - Add a reference to the Jira issue in the GitHub issue.

- **Comment Synchronization**: Link Jira and GitHub issue comments for better communication and collaboration.
    - Convert GitHub markdown to Jira markup for consistent formatting.
    - Append a reference to the GitHub comment within the Jira comment.

## Getting Started

### Installation

1. Copy the `workflows` directory into your project repository.

### Configuration

1. Add the following secrets to your GitHub project:
    - `JIRA_BASE_URL`: Your Jira instance's URL (e.g., `https://mycompany.atlassian.net`).
    - `JIRA_USER_EMAIL`: The email address associated with the Jira user account that will create and post issues (e.g., `john.doe@example.com`).
    - `JIRA_API_TOKEN`: The Jira user's API token.

2. Set the `JIRA_PROJECT_KEY` environment variable in your GitHub project (e.g., `MYPROJ` if your Jira tickets are formatted like `MYPROJ-123`).

### Additional Setup

1. Enable "Autolink references" in your GitHub project settings and use your Jira project key (e.g., `MYPROJ`) as the "Reference prefix".

Now you're all set! Enjoy seamless GitHub and Jira integration with improved collaboration and project management.
