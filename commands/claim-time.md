---
description: Commands for setting claim time to roles.
---

# Claim time

## Adding/removing claimtime
``\

## _**claimtime add**_

`a!claimtime add <role> <claim time> [override]`\

``Adds claim time for a role.

| Argument              | Description                       | Example              |
| --------------------- | --------------------------------- | -------------------- |
| role (required)       | The role to add claim time to     | @role \| 'role name' |
| claim time (required) | The duration of claim time to add | 10s \| 2m \| 5s      |
| override              | Whether to override other roles   | True \| False        |

## _claimtime remove_

`a!claimtime remove <role>`

Deletes claim time for the given role.

| Argument        | Description                        | Example              |
| --------------- | ---------------------------------- | -------------------- |
| role (required) | The role to delete claim time from | @role \| 'role name' |

## _claimtime_

`a!claimtime [user]`

Shows total claim time for a user.
