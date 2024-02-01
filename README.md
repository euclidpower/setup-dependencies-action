# euclidpower/setup-dependencies-action

Reduce the duplication when setting up jobs.

This tool allows you to setup ruby, nodejs and playwright.

# How to use it

```yml
jobs:
  your-new-job:
    name: A descriptive name
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4

      - uses: euclidpower/setup-dependencies-action@v3
        with:
          cache_playwright: true # optional, defaults to "0"

```

# Development
1. Clone the repo
2. Write your changes
3. Create a commit
4. Add a new tag, for example for "v4": `git tag -a -f -m "A description of this new release" v4`
5. Push the tags to origin
6. Confirm the changes work as expected in your codebase. If they don't, you can delete the tag and repeat the process from step 3
