---
name: Hello Agent
on:
  workflow_dispatch:
permissions:
  contents: read
  issues: read
safe-outputs:
  create-issue:
    max: 1
  add-comment:
    max: 1
---

## Task

Search the open issues in this repository.
Find the issue with the most 👍 reactions.
Post a comment on that issue saying:
"This issue has the most community support! We'll prioritise it in our next planning session."

If there are no open issues, create one titled "Community Voting Test" and post the same comment.
