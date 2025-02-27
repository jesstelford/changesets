# @changesets/cli

## 1.3.0

### Minor Changes

- [e55fa3f0](https://github.com/changesets/changesets/commit/e55fa3f0) [#92](https://github.com/changesets/changesets/pull/92) Thanks [@highvoltag3](https://github.com/highvoltag3)! - Catch Promise rejection on SIGINT and exit gracefully
- [94267ff3](https://github.com/changesets/changesets/commit/94267ff3) [#106](https://github.com/changesets/changesets/pull/106) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Improve 2FA support for publishing:

  - Prompt for an OTP code when required
  - Add `--otp` option to release command

### Patch Changes

- [a700de81](https://github.com/changesets/changesets/commit/a700de81) [#104](https://github.com/changesets/changesets/pull/104) Thanks [@Noviny](https://github.com/Noviny)! - Fix auto-generated documentation to point outwards to changesets repo to stop it going stale
- [94267ff3](https://github.com/changesets/changesets/commit/94267ff3) [#106](https://github.com/changesets/changesets/pull/106) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Inline last usages of bolt
- [d4bbab4e](https://github.com/changesets/changesets/commit/d4bbab4e) [#91](https://github.com/changesets/changesets/pull/91) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Convert some internals to TypeScript
- [fc32bc11](https://github.com/changesets/changesets/commit/fc32bc11) [#94](https://github.com/changesets/changesets/pull/94) Thanks [@Noviny](https://github.com/Noviny)! - Better Docs in readme

- Updated dependencies [cbb2c953]:
  - get-workspaces@0.4.0

## 1.2.0

### Minor Changes

- [16fde2e0](https://github.com/changesets/changesets/commit/16fde2e0) [#75](https://github.com/changesets/changesets/pull/75) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Use [enquirer](https://github.com/enquirer/enquirer) instead of inquirer for asking questions because it's smaller, faster and prettier.
  Change bump type questions from asking for each bump type individually per package to asking users to two questions where the user selects what packages should have major and minor bumps and the packages left are assumed to be patch bumps. This dramatically cuts down the amount of time it takes to create a changeset with a large number of packages.

  ![example of using the CLI with the new questions](https://user-images.githubusercontent.com/11481355/58873398-a1c4de80-8709-11e9-80e8-16061e395b15.gif)

### Patch Changes

- [20da7747](https://github.com/changesets/changesets/commit/20da7747) [#66](https://github.com/changesets/changesets/pull/66) Thanks [@Noviny](https://github.com/Noviny)! - Update package.json field so each links into its own package
- [29ff34ed](https://github.com/changesets/changesets/commit/29ff34ed) [#82](https://github.com/changesets/changesets/pull/82) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Limit the number of rows the package selection question takes up so that the question is still visible in repos with a very large number of packages

  ![changeset package question in atlaskit](https://user-images.githubusercontent.com/11481355/59012109-ff783880-8879-11e9-9b68-77ab672921fa.png)

- [ef9be2df](https://github.com/changesets/changesets/commit/ef9be2df) [#81](https://github.com/changesets/changesets/pull/81) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Fix tables in status command from flowing over to the next line

  ![changeset status --verbose output](https://user-images.githubusercontent.com/11481355/59011589-875d4300-8878-11e9-9e69-cada41f83261.png)

- [91000292](https://github.com/changesets/changesets/commit/91000292) [#78](https://github.com/changesets/changesets/pull/78) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Fix misaligned CLI messages

## 1.1.5

### Patch Changes

- [7fa42641](https://github.com/changesets/changesets/commit/7fa42641) [#61](https://github.com/changesets/changesets/pulls/61) Thanks [@Noviny](https://github.com/Noviny)! - When bumping, run prettier over the changelog file.

  If you want this option turned off, add `disabledLanguage: ["markdown"] to your prettier config.

  - [6dc510f4](https://github.com/changesets/changesets/commit/6dc510f4) [#62](https://github.com/changesets/changesets/pulls/62) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Add butterfly emoji prefix to CLI output

## 1.1.4

### Patch Changes

- [83ba6d3f](https://github.com/Noviny/changesets/commit/83ba6d3f) - Convert various modules to TypeScript
- [a966701d](https://github.com/Noviny/changesets/commit/a966701d) - Add repository information to package.json
- [c00e65ef](https://github.com/Noviny/changesets/commit/c00e65ef) - Fix bug where unprovided command line options overrode the config file, leading to incorrect states
- [8d2e700c](https://github.com/Noviny/changesets/commit/8d2e700c) - Remove unused function parseChangesetCommit
- [7399648d](https://github.com/Noviny/changesets/commit/7399648d) - Make ids human readable

- Updated dependencies [83ba6d3f]:
  - get-workspaces@0.3.0

## 1.1.3

### Patch Changes

- [67db935d](https://github.com/Noviny/changesets/commit/67db935d) - Fix release without built files

## 1.1.2

### Patch Changes

- [c6f1c7b7](https://github.com/Noviny/changesets/commit/c6f1c7b7) [#46](https://github.com/Noviny/changesets/pulls/46) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Convert a file to TypeScript
- [9fe9ecff](https://github.com/Noviny/changesets/commit/9fe9ecff) [#45](https://github.com/Noviny/changesets/pulls/45) Thanks [@Noviny](https://github.com/Noviny)! - Print out the last changes.md path in terminal as last step of adding a changeset
- [61ac9ce7](https://github.com/Noviny/changesets/commit/61ac9ce7) [#42](https://github.com/Noviny/changesets/pulls/42) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Make "All changed packages" option first in package list

- Updated dependencies [355b4d00]:
  - get-workspaces@0.2.0

## 1.1.1

### Patch Changes

- [b93d04a2](https://github.com/Noviny/changesets/commit/b93d04a2) - Consume get-workspaces as dependency
- [079eabae](https://github.com/Noviny/changesets/commit/079eabae) [#33](https://github.com/Noviny/changesets/pulls/33) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Fix a bug with linked packages where it would break if there was a linked package that didn't have a changeset

- Updated dependencies [b93d04a2]:
  - get-workspaces@0.1.0

## 1.1.0

### Minor Changes

- [6929624b](https://github.com/Noviny/changesets/commit/6929624b) [#27](https://github.com/Noviny/changesets/pulls/27) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Add linked packages/lockstep

## 1.0.1

### Patch Changes

- 9435d886: Fix binary and published files

## 1.0.0

### Major Changes

- 51c8b0d6: Remove `noChangelog` flag in favor of `updateChangelog` flag (default behaviour remains the same).

  If you were using this custom flag, you will need to replaces `noChangelog: true` with `updateChangelog: false`

- 51c8b0d6: Rename commands from @atlaskit/build-releases

  We are no longer mirroring the names from npm/yarn commands, so it is easy to write package scripts
  for each command without footguns. The functionality of the commands remains the same. In addition,
  the binary has been changed to `changeset`.

  The new names are:

  - `build-releases initialize` => `changeset init` (for ecosystem consistency)
  - `build-releases changeset` => `changeset` (default command). You can also run `changeset add`
  - `build-releases version` => `changeset bump`
  - `build-releases publish` => `changeset release`

  The function of these commands remains unchanged.

  - 51c8b0d6: Change format of changelog entries

  Previously changelog entries were in the form of:

  ```md
  ## 2.1.0

  - [patch] Allows passing --public flag for publishing scoped packages [159c28e](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/159c28e)
  - [minor] Changes changelogs to be opt out rather than opt in [f461788](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/f461788)
  ```

  which doesn't take into account the importance of particular entries. We are moving to an ordered system for changelog
  entries, and to match this, we are updating the headings we use to the following format:

  ```md
  ## 2.1.0

  ### Minor

  - Allows passing --public flag for publishing scoped packages [159c28e](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/159c28e)

  ### Patch

  - [minor] Changes changelogs to be opt out rather than opt in [f461788](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/f461788)
  ```

  This changes the format of the default `getReleaseLine` from

  ```js
  const getReleaseLine = async (changeset, versionType) => {
    const indentedSummary = changeset.summary
      .split("\n")
      .map(l => `  ${l}`.trimRight())
      .join("\n");

    return `- [${versionType}] ${changeset.commit}:\n\n${indentedSummary}`;
  };
  ```

  to

  ```js
  const getReleaseLine = async (changeset, type) => {
    const [firstLine, ...futureLines] = changeset.summary
      .split("\n")
      .map(l => l.trimRight());

    return `- ${changeset.commit}: ${firstLine}\n${futureLines
      .map(l => `  ${l}`)
      .join("\n")}`;
  };
  ```

  You will end up with some odd changelog entries if you do not update your release line.

### Minor Changes

- 51c8b0d6: Support non-bolt repositories

  Changesets have been expanded to support:

  - bolt repositories
  - yarn workspaces-based repositories
  - single package repositories.

  Currently **not** supported: bolt repositories with nested workspaces.

  To do this, functions that call out to bolt have been inlined, and obviously marked
  within the file-system. In addition, the `get-workspaces` function has undergone
  significant change, and will be extracted out into its own package soon.

  This is to support other tools wanting this level of inter-operability.

  If plans to modularize bolt proceed, we may go back to relying on its functions.

  This should have no impact on use.

  - 51c8b0d6: Add 'select all' and 'select all changed' options, to make mass-bumping easier.
  - eeb4d5c6: Add new command: `status` - see Readme for more information

# @atlaskit/build-releases - legacy changelog

## 3.0.3

- [patch][c87337f](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/c87337f):

  - The version command now removes empty folders before it starts. This should prevent a race condition in CI

## 3.0.2

- [patch][f7b030a](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/f7b030a):

  - Fixes potential infinite loop in parseChangesetCommit

## 3.0.1

- [patch][494c1fe](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/494c1fe):

  - Update git commit message to match previous tooling.

## 3.0.0

- [major][44ec8bf" d](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/44ec8bf"
  d):

  Changesets now use local file system - this has several effects:

  1. Changesets will no longer automatically create a commit. You will need to add and commit the files yourself.
  2. Changesets are easier to modify. You should ONLY modify the changes.md file (_Not changes.json_).
  3. There will be a new directory which is `.changeset`, which will hold all the changesets.

  Apart from these changes, your process using this should not have changed.

  Changeset now accepts skipCI flag, where previously release commits automatically skipped CI. i.e.

  ```
  yarn build-releases version --skipCI
  ```

  **Breaking**: Changeset and version commands now accept `--commit` flag which makes them commit automatically (previously this was the default behaviour). Otherwise, these commands simply make the file-system changes.

  ```
  yarn build-releases changeset --commit
  ```

  We also introduce the `intitialize` command. See the package [README.md](https://www.npmjs.com/package/@atlaskit/build-releases) for more details about this.

## 2.1.3

- [patch] Bumps bolt version to get some bug fixes around publishing [493f5f7](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/493f5f7)

## 2.1.2

- [patch] Pulls in fix in bolt causing publishing to fail when running a yarn subprocess (see boltpkg/bolt #189) [2b36121](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/2b36121)

## 2.1.1

- [patch] Fixes bug where empty summaries would cause a changeset to not get found [25b30bf](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/25b30bf)

## 2.1.0

- [minor] Allows passing --public flag for publishing scoped packages [159c28e](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/159c28e)
- [minor] Changes changelogs to be opt out rather than opt in [f461788](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/f461788)

## 2.0.0

- [major] Completely refactors build-releases to be externally consumable 8458ef7](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/8458ef7)

## 1.28.2

- [patch] Bug fix and better error messages for changeset error [7f09b86](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/7f09b86)

## 1.28.1

- [patch] update flow dep, fix flow errors [722ad83](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/722ad83)

## 1.28.0

- [minor] Adds tagging to releases [34c64fd](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/34c64fd)

## 1.27.0

- [minor] Splits out and exposes flattenChangesets function [5ee5f74](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/5ee5f74)

## 1.26.0

- [minor] Lots of new features (consider this package unstable and only for use internally) [7cdf2e6](https://bitbucket.org/atlassian/atlaskit-mk-2/commits/7cdf2e6)
