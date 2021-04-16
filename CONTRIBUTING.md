# Contributing
Please read this document before adding code to the repository.

## Labels
The labels are used to be able to easily find and organise issues. There are several categories:

### Issue Type
These labels ("devops", "bug", "documentation", "feature") are the type of issue that has been 
raised and are used in the branch naming convention.

### Related Pages
These labels have the suffix `page` and are used to link issues to specific views of the application.

### Size
These labels estimate the complexity and estimated time to completion of issues to track velocity 
for each sprint.

### Misc.
The remaining labels are used for filtering and searching. The descriptions can be found in the
[repository](https://github.com/JOSA-Tech/JOSA-mobile/labels) or by hovering over the labels in an 
issue.

## Workflow
1. Clone/Pull staging branch for most recent updates
2. Assign yourself to an issue
3. Create a local branch following the branch naming convention
    * `<issue id>`-`<issue type>`-`<short>`-`<description>`
    * eg. `1-documentation-example-issue`
4. Implement changes
5. Run flutter analyze command to ensure project passes linting.
6. Run flutter formatter on source code to maintain codebase formatting.
  * Either run `flutter format -l 120 lib`
  * Or setup your text-editor to automatically format on save with line length 120
7. Push branch to remote with `--set--upstream` flag
    * eg. `git push --set-upstream origin <branch name>`
8. Start pull request targeting the staging branch using the template
9. Address any comments brought up in the review
10. Once the code has passed review, merge the branch

## Code conventions
This project follows [dart best practices](https://dart.dev/guides/language/effective-dart/style) 
and flutter formatting
