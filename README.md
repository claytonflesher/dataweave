# Exercism Dataweave Track

Exercism Exercises in Dataweave

## Setup

The exercises currently target Dataweave versions 2.X. Detailed installation instructions can be found at 
[https://developer.mulesoft.com/tutorials-and-howtos/dataweave/dataweave-extension-vscode-getting-started/](https://developer.mulesoft.com/tutorials-and-howtos/dataweave/dataweave-extension-vscode-getting-started/)
## Testing

---

> It is recommended to test BEFORE submitting a PR. It will test your submission, ensure
> that the repository builds as a whole, and help guard against unintentional, unrelated changes.

---

### Test Exercises

To test all of the exercises against their example solution, you can run `bin/test_exercises.sh`:

```shell
$ ./bin/test_exercises.sh
Testing: accumulate Pass
Testing: acronym Pass
...
Testing: zipper Pass
--------------------------------------------------------------------------------
93/93 tests passed.
```

This will take some time.

To only test some exercises, run:

```shell
$ ./bin/test_exercises.sh word-count zebra-puzzle
Testing: word-count Pass
Testing: zebra-puzzle Pass
--------------------------------------------------------------------------------
2/2 tests passed.
```

### Dialyzer

To run dialyzer on all exercises, run `./bin/dialyzer_check.sh`. It might take a really long time the first time you run it. It will also be run for you by Github Actions as part of the PR check.

### Code and document formatting

To check formatting of all exercises and all documents, run `./bin/check_formatting.sh`. It will also be run for you by Github Actions as part of the PR check.

### Track linting

[`configlet`](https://github.com/exercism/configlet) is an Exercism-wide tool for working with tracks. You can download it by running:

```shell
$ ./bin/fetch-configlet
```

Run its `lint` command to verify if all exercises have all the necessary files and if config files are correct:

```shell
$ ./bin/configlet lint

The `exercises.practice.slug` value is `transpose 🙂`, but it must be a lowercase and kebab-case string:
/Users/cflesher/exercism/dataweave/config.json

Configlet detected at least one problem.
For more information on resolving the problems, please see the documentation:
https://github.com/exercism/docs/blob/main/building/configlet/lint.md
```

## Contributing Guide
