# Google Workspace Operations

This directory contains Google Workspace admin operation specifications that are reviewed and approved via Pull Requests.

## Structure

Each operation is stored as a JSON file with the following naming convention:
- `{timestamp}-{operation-type}-{id}.json`

## Workflow

1. Admin requests a change via the webapp
2. System generates an operation spec file and creates a PR
3. Approvers review the PR
4. Once merged, the operation is automatically executed
5. Results are logged back to the webapp

## Operation Types

- `user.create` - Create new user
- `user.suspend` - Suspend user account  
- `user.restore` - Restore suspended user
- `user.delete` - Delete user account
- `group.create` - Create new group
- `group.delete` - Delete group
- `group.addMember` - Add member to group
- `group.removeMember` - Remove member from group
