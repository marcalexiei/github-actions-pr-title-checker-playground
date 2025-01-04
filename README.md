# github-actions-pr-title-checker

Trying out a simple action workflow to validate PR titles.

> [!NOTE]
> No need for third party actions / libraries

---

> [!TIP]
> To provide a user friendly messages this workflow uses
> Github annotations.
>
> Specifically [notice](https://docs.github.com/en/actions/writing-workflows/choosing-what-your-workflow-does/workflow-commands-for-github-actions#setting-a-notice-message) and [error](https://docs.github.com/en/actions/writing-workflows/choosing-what-your-workflow-does/workflow-commands-for-github-actions#setting-an-error-message) types
>
> Why use annotations instead of adding a comment on the PR?
> To add a comment the workflow must have a [pull_request_target](https://docs.github.com/en/actions/writing-workflows/choosing-when-your-workflow-runs/events-that-trigger-workflows#pull_request_target) trigger
> to properly inherit a `GITHUB_TOKEN` with the proper permissions.
>
> Annotations do not require this kind of permissions

## Credits

The bash validation has been inspired by [sh-conventional-commits](https://github.com/joaobsjunior/sh-conventional-commits/blob/main/commit-msg)
