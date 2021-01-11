# Github Actions

### turn on debug mode in github actions

https://docs.github.com/en/free-pro-team@latest/actions/managing-workflow-runs/enabling-debug-logging#enabling-runner-diagnostic-logging

### supported scripts

https://docs.github.com/en/free-pro-team@latest/actions/reference/workflow-syntax-for-github-actions#using-a-specific-shell

### action marketplace

https://github.com/marketplace?type=actions

### on pul_request run on open, reopen and synchronize

https://docs.github.com/en/free-pro-team@latest/actions/reference/events-that-trigger-workflows

### schedule

Cron syntax has five fields separated by a space, and each field represents a unit of time.

┌───────────── minute (0 - 59)
┌───────────── hour (0 - 23)
│ │ ┌───────────── day of the month (1 - 31)
│ │ │ ┌───────────── month (1 - 12 or JAN-DEC)
│ │ │ │ ┌───────────── day of the week (0 - 6 or SUN-SAT)
│ │ │ │ │  
│ │ │ │ │
│ │ │ │ │

---

You can use these operators in any of the five fields:

Operator Description Example

- Any value \* \* \* \* _ runs every minute of every day.
  , Value list separator 2,10 4,5 _ \* \* runs at minute 2 and 10 of the 4th and 5th hour of every day.

* Range of values 0 4-6 \* _ * runs at minute 0 of the 4th, 5th, and 6th hour.
  / Step values 20/15 * _ \* \* runs every 15 minutes starting from minute 20 through 59 (minutes 20, 35, and 50).

#### good tool

https://crontab.guru/

#### Manual events

You can manually trigger workflow runs. To trigger specific workflows in a repository, use the workflow_dispatch event. To trigger more than one workflow in a repository and create custom events and event types, use the repository_dispatch event.

### filtering

https://docs.github.com/en/free-pro-team@latest/actions/reference/workflow-syntax-for-github-actions#filter-pattern-cheat-sheet

can filter on branches tags paths

### env

https://docs.github.com/en/free-pro-team@latest/actions/reference/environment-variables

### encrypt env

https://github.com/Ivan-Mitkov/github_actions/settings/secrets/actions

https://docs.github.com/en/free-pro-team@latest/actions/reference/encrypted-secrets

### Authentication in a workflow

https://docs.github.com/en/free-pro-team@latest/actions/reference/authentication-in-a-workflow

### encrypt files

https://docs.github.com/en/free-pro-team@latest/actions/reference/encrypted-secrets

encrypt files on local machine

https://gnupg.org/download/index.html

https://www.gnupg.org/gph/de/manual/r1023.html

### expressions and context

https://docs.github.com/en/free-pro-team@latest/actions/reference/context-and-expression-syntax-for-github-actions
