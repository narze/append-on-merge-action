# append-on-merge-action

See <https://github.com/narze/append_on_merge>

Github Action to append to file only when PR in a specific folder is merged, preventing conflicts

## Workflow

- Specify input folder e.g. `/input`.
- Contributors create file within input folder with different file names.
- Contributors then submit non conflicting Pull Requests, since all files have different names.
- When PRs merged, the action will append the target file, then delete the input file, or move the file to another folder e.g. `/processed`
- (Optional) The action could preview how the target file will look like after appending using comments within PRs.
