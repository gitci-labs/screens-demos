# Screens Demos

Demo projects for GitCI Screens.

Included demos:

- `demos/minimal`: target-aware scene variants, a project-local template pack, palette-mapped theme variables, and a spanned scene example.
- `demos/todo-basic`: a straightforward productivity app scene set for iPhone, iPad, and Mac.
- `demos/reader-immersive`: a reading/study app scene set with target-specific feature closeups.
- `demos/pro-mac-app`: a dark-mode pro workflow scene set spanning mobile, tablet, and desktop.

CI checks the demos against the current `gitci-labs/screens` CLI and bundled template pack, then uploads zipped screenshot builds as workflow artifacts. Locally, from the private `gitci-dev` meta repo, you can run:

```sh
GITCI_SCREENS_JS_WORKSPACE="$PWD/screens/js" \
GITCI_SCREENS_TEMPLATES_ROOT="$PWD/screens/templates/gitci/screens" \
screens/.build/debug/gitci-screens export screens-demos/demos/todo-basic --strict
```
