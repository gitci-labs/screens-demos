# Screens Demos

Demo projects for GitCI Screens.

`demos/minimal` is a fake app screenshot project with a `gitci/screens` directory, target-aware scene variants, a project-local template pack, palette-mapped theme variables, and a spanned scene example.

CI checks the demo against the current `gitci-labs/screens` CLI and bundled template pack. Locally, from the private `gitci-dev` meta repo, you can run:

```sh
GITCI_SCREENS_JS_WORKSPACE="$PWD/screens/js" \
GITCI_SCREENS_TEMPLATES_ROOT="$PWD/screens/templates/gitci/screens" \
screens/.build/debug/gitci-screens build screens-demos/demos/minimal
```
