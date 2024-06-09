# gha-example

`gha-example` is a repository that showcases the reusable [`cmaster11/gha`](https://github.com/cmaster11/gha) GitHub
Actions builder workflows.

Important files:

- The [`build.yml`](.github/workflows/build.yml) workflow reuses the
  reusable [`cmaster11/gha/.github/workflows/build.yml`](https://github.com/cmaster11/gha/blob/main/.github/workflows/build.yml)
  to trigger the whole GitHub Actions build pipeline.
- The [`actions/action-test/action.yml`](actions/action-test/action.yml) file defines a TypeScript test
  action ([`index.ts`](actions/action-test/index.ts)) and
  the [`.github/workflows/test-action-test.yml`](.github/workflows/test-action-test.yml) contains its test logic.

Whenever you open a PR and edit the [actions/action-test](actions/action-test) folder, the build process is then triggered.