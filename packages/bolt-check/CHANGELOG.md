# bolt-check

## 0.4.0

### Minor Changes

- [23ee7d64](https://github.com/changesets/changesets/commit/23ee7d64) [#108](https://github.com/changesets/changesets/pull/108) Thanks [@Blasz](https://github.com/Blasz)! - Add javascript API for bolt-check. The API currently contains check and fix commands.

- Updated dependencies [cbb2c953]:
  - get-workspaces@0.4.0

## 0.3.0

### Minor Changes

- [3d2f023f](https://github.com/changesets/changesets/commit/3d2f023f) [#77](https://github.com/changesets/changesets/pull/77) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Stop checking peerDependencies because peerDependencies are very different to dependencies and devDependencies. They generally need different ranges than what dependencies and devDependencies have and they also don't affect what version of a dependency is installed. bolt and bolt-check already only check the devDep version if there's a package that is a devDep and peerDep (and similar for other cases) so this doesn't affect checking, only auto fixing.
- [f71188cd](https://github.com/changesets/changesets/commit/f71188cd) [#74](https://github.com/changesets/changesets/pull/74) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Add check banning devDependencies in root package.jsons

### Patch Changes

- [20da7747](https://github.com/changesets/changesets/commit/20da7747) [#66](https://github.com/changesets/changesets/pull/66) Thanks [@Noviny](https://github.com/Noviny)! - Update package.json field so each links into its own package

## 0.2.0

### Minor Changes

- [df63e9c0](https://github.com/changesets/changesets/commit/df63e9c0) [#64](https://github.com/changesets/changesets/pulls/64) Thanks [@Noviny](https://github.com/Noviny)! - Add '--fix' command - a very useful new feature

## 0.1.0

### Minor Changes

- [a966701d](https://github.com/Noviny/changesets/commit/a966701d) - Initial Release
