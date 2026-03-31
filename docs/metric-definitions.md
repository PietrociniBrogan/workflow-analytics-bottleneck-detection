# Metric Definitions

## 1. Workflow Cycle Time

Definition: Total time from workflow submission to workflow completion.
Business Value: Shows how long work takes end to end.
Formula Idea: completed_at - submitted_at
Notes: Exclude workflows not yet completed from average completed cycle time.

## 2. Stage Cycle Time

Definition: Time spent in each workflow stage.
Business Value: Identifies bottlenecks in the process.
Formula Idea: stage_exit_timestamp - stage_entry_timestamp
Notes: Requires event ordering to be reliable.

## 3. Backlog Count

Definition: Number of workflows currently open and not completed.
Business Value: Shows work in progress and pressure on the system.
Formula Idea: count of workflows with status not in completed/closed states

## 4. Reopen Rate

Definition: Percentage of workflows or issues reopened after being resolved or closed.
Business Value: Signals quality problems or incomplete resolution.
Formula Idea: reopened_items / completed_items
Notes: Must define exactly what qualifies as reopened.

## 5. On-Time Completion Rate

Definition: Percentage of completed workflows finished on or before target due time.
Business Value: Measures deadline compliance.
Formula Idea: completed_on_time / total_completed
Notes: Requires due date or target completion timestamp.
