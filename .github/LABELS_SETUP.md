# GitHub Labels Setup Guide

This document provides instructions for setting up the recommended labels for the My Sailing Log feedback repository.

## Required Labels

### Status Labels
Create these labels to track issue status:

- **needs-triage** - `#f9ca24` (Yellow) - New issue awaiting review
- **in-progress** - `#6c5ce7` (Purple) - Currently being worked on
- **triaged** - `#00b894` (Green) - Reviewed and approved for development
- **blocked** - `#e17055` (Orange) - Waiting on external dependencies
- **wont-fix** - `#636e72` (Gray) - Will not be implemented

### Priority Labels
Create these labels to indicate priority levels:

- **priority-critical** - `#d63031` (Red) - Blocking issue, needs immediate attention
- **priority-high** - `#e84393` (Pink) - Important feature or bug
- **priority-medium** - `#0984e3` (Blue) - Nice to have
- **priority-low** - `#00b894` (Green) - Future consideration

### Type Labels
Create these labels to categorize issues:

- **bug** - `#d63031` (Red) - Something isn't working
- **feature-request** - `#00b894` (Green) - New functionality
- **enhancement** - `#6c5ce7` (Purple) - Improvement to existing feature
- **documentation** - `#74b9ff` (Light Blue) - Documentation improvements

### Special Labels
Create these labels for specific purposes:

- **good-first-issue** - `#00cec9` (Teal) - Good for new contributors
- **help-wanted** - `#fd79a8` (Pink) - Community help needed
- **duplicate** - `#636e72` (Gray) - Duplicate of another issue

## How to Create Labels

1. Go to your repository: `https://github.com/delwinbest/mysailinglog-feedback`
2. Click on the "Issues" tab
3. Click on "Labels" on the right sidebar
4. Click "New label" for each label above
5. Enter the label name and select the corresponding color
6. Click "Create label"

## Project Board Setup

Create a project board to visualize issue workflow:

### Board Name
"My Sailing Log - Issue Management"

### Columns (in order)
1. **Backlog** - New issues that need triage
2. **Needs Triage** - Issues requiring review and prioritization
3. **In Progress** - Issues currently being worked on
4. **In Review** - Issues completed and awaiting review
5. **Done** - Completed and deployed issues

### Automation Rules
Set up these automation rules for the project board:

1. **Auto-move to "Needs Triage"** when label `needs-triage` is added
2. **Auto-move to "In Progress"** when label `in-progress` is added
3. **Auto-move to "Done"** when issue is closed

## Issue Workflow

### Bug Reports
1. Issue created with `bug` and `needs-triage` labels
2. Team reviews and assigns priority label
3. Issue moved to appropriate priority column
4. Development begins - issue gets `in-progress` label
5. Issue closed when fix is deployed

### Feature Requests
1. Issue created with `feature-request` and `needs-triage` labels
2. Team reviews and assigns priority label
3. Community voting period (use GitHub reactions)
4. Approved features get `triaged` label
5. Development begins - issue gets `in-progress` label
6. Issue closed when feature is deployed

## GitHub Embed Widget Configuration

The application uses GitHub embed widgets with these configurations:

### Help Center Page
```html
<iframe
  src="https://github.com/delwinbest/mysailinglog-feedback/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc"
  width="100%"
  height="600"
  frameBorder="0"
  title="GitHub Issues"
/>
```

### Features Page
```html
<iframe
  src="https://github.com/delwinbest/mysailinglog-feedback/issues?q=is%3Aissue+is%3Aopen+label%3Afeature-request+sort%3Aupdated-desc"
  width="100%"
  height="600"
  frameBorder="0"
  title="Feature Requests"
/>
```

## Issue Templates

The repository includes two issue templates:

1. **Bug Report** (`.github/ISSUE_TEMPLATE/bug_report.yml`)
   - Automatically applies `bug` and `needs-triage` labels
   - Collects browser, device, steps to reproduce, expected vs actual behavior

2. **Feature Request** (`.github/ISSUE_TEMPLATE/feature_request.yml`)
   - Automatically applies `feature-request` and `needs-triage` labels
   - Collects priority, use case, problem statement, proposed solution

## Best Practices

1. **Always use labels** - Every issue should have appropriate labels
2. **Keep descriptions detailed** - Help developers understand the issue
3. **Use reactions for voting** - 👍 for support, 👎 for opposition
4. **Link related issues** - Use "Closes #X" in commit messages
5. **Update status regularly** - Keep labels current as work progresses
6. **Close completed issues** - Mark issues as closed when work is done

## Automation Scripts

Consider setting up GitHub Actions for:

1. **Auto-labeling** - Automatically apply labels based on issue content
2. **Status updates** - Update labels when pull requests are merged
3. **Reminder bots** - Notify when issues have been stale for too long
4. **Metrics collection** - Track issue resolution times and trends

## Contact

For questions about this setup, create an issue in this repository or contact the development team.