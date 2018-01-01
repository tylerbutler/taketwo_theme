# taketwo_theme

## Building

To build, clone the project and run:

```text
npm install
npm install --only=dev
```

Then run the actual build using gulp:

```text
gulp build
```

If you make changes to the Semantic UI config, you'll need to build Semantic UI itself, because the standard theme build task doesn't build Semantic UI to keep builds fast. But it's easy to build when needed using gulp:

```text
gulp buildsemui
```

After any changes, a full build (meaning `gulp buildsemui` followed by `gulp build`) should be run and the results should be committed. Yup, that means a lot of duplicates and unnecessary stuff is committed.

Long term I want to make this better but that's a problem for Future Tyler.
