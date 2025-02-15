# Intermittent Expo CLI Build Failures

This repository demonstrates an unusual issue encountered with the Expo CLI build process. The build process fails intermittently, providing vague error messages that offer little insight into the root cause.  The problem is inconsistent, sometimes building successfully on subsequent attempts.

## Steps to Reproduce

1. Clone this repository.
2. Install the dependencies: `npm install` or `yarn install`
3. Attempt to build the project using `expo build:android` or `expo build:ios`. Note that the build may succeed or fail inconsistently.

## Troubleshooting Steps Attempted

* Clearing the Expo cache (`expo start --clear`)
* Reinstalling node modules (`npm install` or `yarn install`)
* Creating a new Expo project from scratch
* Checking the Expo CLI and Node.js versions
* Restarting the machine

None of these steps consistently resolved the issue.

## Solution (bugSolution.js)

The solution involves checking the system's temporary folders for any lingering build files, and exploring more nuanced build options.