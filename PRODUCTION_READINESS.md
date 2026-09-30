# Production readiness plan — GitHub slideshow

Assessment date: 2026-09-30. Estimated readiness: **30%** if the goal is a maintained public slideshow site. As an educational GitHub Learning Lab repository, it may already have served its purpose; a commercial production target has not been defined.

## Evidence
- Repository is a GitHub Learning Lab reveal.js/Jekyll template with one intro slide and an existing `script/cibuild`.
- `node_modules/reveal.js` is committed, the Jekyll dependency set is old, and no GitHub Actions workflow is present in the file tree.
- README describes the historical learning exercise, with no current publishing or maintenance instructions.

## Work completed on this branch
- Added this scope and production checklist; clarified the README.

## Remaining, in priority order
1. Decide whether the repository should remain an archived learning exercise or become a public presentation.
2. If maintained, replace the template author/title and create actual slides with accessible text and images.
3. Remove committed dependency artifacts after establishing a reproducible dependency installation; update and lock supported Jekyll/reveal.js versions.
4. Run `script/cibuild` on supported Ruby, fix failures, then add CI.
5. Configure and smoke test deployment, navigation, mobile display, and link validity.
