# How to contribute

There are many ways to contribute to nodecg-io: logging bugs, submitting pull requests, reporting issues, and creating suggestions.

First you'll need a installation of nodecg-io. Please refer to the [installation guide](../getting_started/install.md) but
instead of using our repository you might want to fork the nodecg-io repository to your GitHub account and clone your fork.

## Build

### VsCode

In `Vscode` you can start the build task with
<kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>B</kbd> (<kbd>CMD</kbd>+<kbd>Shift</kbd>+<kbd>B</kbd> on macOS).
The incremental builder will do an initial full build.  
The watch builder will watch for file changes and compile those changes incrementally, giving you a fast, iterative coding experience.
It will even stay running in the background if you close VS Code.
You can resume it by starting the build task with
<kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>B</kbd> (<kbd>CMD</kbd>+<kbd>Shift</kbd>+<kbd>B</kbd>) again.  
ou can kill the build task by pressing <kbd>Ctrl</kbd>+<kbd>D</kbd> in the task terminal (<kbd>CMD</kbd>+<kbd>D</kbd> on macOS.  
Errors and warnings will be shown in the status bar at the bottom left of the editor. You can view the error list using `View | Errors and Warnings` or pressing <kbd>Ctrl</kbd>+<kbd>P</kbd> and then <kbd>!</kbd> (<kbd>CMD</kbd>+<kbd>P</kbd> and <kbd>!</kbd> on macOS)

### Terminal

You can also use you terminal to build nodecg-io:

```
cd path/to/nodecg-io
npm run build
```

The watch builder can be activated here too:

```
cd path/to/nodecg-io
npm run watch
```

## Add nodecg-io directory to the nodecg config:

Modify the nodecg configuration in `path/to/nodecg/cfg/nodecg.json`, here is an example config:

```json
{
    "bundles": {
        "paths": ["path/to/nodecg-io", "path/to/nodecg-io/samples"]
    }
}
```

_Note 1:_ This path should point to the root of this repository, not to a bundle inside this repo.

_Note 2:_ The second path to the samples is only required if you want to use a sample plugin.

_Note 3:_ If nodecg doesn't load nodecg-io for some reason you might want to use an absolute path here.

## Run

To test the changes you simply need to start/restart nodecg.

### Automated Testing

> Nothing yet

### Unit Testing

> Nothing yet

## Work Branches

Even if you have push rights on the codeoverflow-org/nodecg-io repository, you should create a personal fork and create feature branches there when you need them. This keeps the main repository clean and your personal workflow cruft out of sight.

## Pull Requests

Occasionally you will want to merge changes in the upstream repository (the official code repo) with your fork.

```
cd path/to/nodecg-io
git checkout master
git pull https://github.com/codeoverflow-org/nodecg-io master
```

Manage any merge conflicts, commit them, and then push them to your fork. Now you can make a pull request from your folk.

### Where to Contribute

After cloning and building the repo, check out the [issues list](https://github.com/codeoverflow-org/nodecg-io/issues). Issues labeled [`help wanted`](https://github.com/codeoverflow-org/nodecg-io/labels/help%20wanted) are good issues to submit a PR for. Issues labeled [`good first issue`](https://github.com/codeoverflow-org/nodecg-io/labels/good%20first%20issue) are great candidates to pick up if you are in the code for the first time. If you are contributing significant changes, please discuss with the assignee of the issue first before starting to work on the issue.

## Packaging

> Maybe in the future

## Suggestions

We're also interested in your feedback. You can submit a suggestion or feature request through the issue tracker. To make this process more effective, we're asking that these include more information to help define them more clearly.

## Discussion Etiquette

In order to keep the conversation clear and transparent, please limit discussion to English and keep things on topic with the issue. Be considerate to others and try to be courteous and professional at all times.
