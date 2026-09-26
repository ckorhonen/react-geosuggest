# Working on react-geosuggest

Read `CONTRIBUTING.md` and `CONVENTIONS.md`. Source is in `src/`, tests and Google
Maps stubs in `test/`, demo sources in `example/src/`, and browser bundles in
`dist/`. Preserve React compatibility and BEM CSS naming.

Use `npm install` in a compatible legacy Node environment; historical CI covers
Node 4 and 5. Installation can run the `prepublish` module build. `npm test` runs
lint, covered unit tests, and coverage reports. `npm run unit-test` is the focused
suite and `npm run lint` the lint gate. `npm run build:module` compiles module
output; `npm run build:browser` rebuilds distribution bundles. There is no
separate typecheck script.

`npm start` builds and serves the demo on port 8000. Tests use Google stubs;
live Places behavior needs an authorized API key and separate browser evidence.
Release scripts can commit and publish the example site, so they are not checks.
Follow contributor requirements for behavior tests and public API documentation.

## Completing changes

Follow existing patterns and carry authorized work through the relevant checks,
repairing failures caused by the change. Choose routine implementation details
directly; ask only when missing information materially changes scope or outcome.
For documentation-only edits, check the diff, referenced paths, and command
accuracy rather than starting application runtimes. If a prerequisite blocks a
check, report the exact blocker and continue independent authorized work. Close
with changed paths, checks actually run and results, and remaining unverified
behavior; distinguish commands inspected from commands executed.
