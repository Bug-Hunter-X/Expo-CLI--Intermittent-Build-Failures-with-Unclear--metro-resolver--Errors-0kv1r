# Expo CLI: Intermittent Build Failures with Unclear `metro-resolver` Errors

This repository demonstrates a bug encountered while using the Expo CLI. The issue involves intermittent build failures with vague error messages related to the `metro-resolver` module.  The error messages provided little to no information about the source of the problem, making debugging difficult.

## Bug Reproduction

1. Clone this repository.
2. Navigate to the project directory.
3. Run `expo start`.
4. Observe the intermittent build failures, often without clear error messages beyond general `metro-resolver` issues.

## Solution

The solution often involved a combination of steps including:
* Cleaning the cache (`expo prebuild --clean`)
* Ensuring all dependencies are up-to-date
* Checking for conflicting dependency versions
* Restarting the Expo CLI and development server
* In rare cases, reinstalling Node modules