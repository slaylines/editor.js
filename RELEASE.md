# Release

## Versioning

Our version tag consists of two versions:

- Version of our modifications of Editor.js.
- Version of Editor.js the modifications are based on.

For example, the initial version we started with is `v1.0.0-ejs-v2.29.1`:

- Version of our modifications is `v1.0.0`.
- The modifications are based on Editor.js `v2.29.1`.

## Upgrading

To upgrade Editor.js version just pull a corresponding tag:

```
git pull editorjs v2.29.1
```

- If upgrade goes smooth then release a new version of the package with Editor.js version bumped.
- If additional integration work has been required make sure to bump the modifications version too.

## Publication

Once all the changes are ready and commited, add a new entry to the `CHANGELOG.md` file, and create a new tag:

```markdown
### v1.0.0-ejs-v2.29.1

- Initial version.
- Add `RELEASE.md` and this `CHANGELOG.md`.
```

```bash
git add -A
git commit -m "Release v1.0.0-ejs-v2.29.1"
git tag v1.0.0-ejs-v2.29.1
git push origin v1.0.0-ejs-v2.29.1
```