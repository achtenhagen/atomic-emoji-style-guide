
# Atomic Emoji Style Guide

**Version 1.1 - December, 2017**

Combining atomic commits with emoji prefixing to create more meaningful commit messages.

## Atomic Commits

- Code reviews are more efficient, because each commit only focuses on **one** single change.
- Bug fixes can be tested more easily since only relevant changes are grouped together.
- Commits can be rolled back without leaving the system in an inconsistent state.

## Emoji Prefixing

- The use of emoji allows the developer to foresee how the commit changes the code.
- Associating a single emoji with the type of commit helps the developer make more focused changes.
- Adopting this style guide supports consistency and uniformity, resulting in cleaner repositories, prettier git logs and happier devs! ⚛️ + 😜 = ❤️

## Commit Message Structure

`[ Emoji ]` + `[ Title ]` + `[ Description ]`

`[ Emoji ]` is defined as one of the following items below:

| Emoji | Description |
|:-----:| ----------- |
|  🐛   | The commit introduces a bug fix, which ideally references the commit where the bug was introduced. |
|  🔨   | The commit refactors existing code, without changing its functionality. |
|  💅   | The commit introduces a new style or style change, which must not affect the logic of any existing code. |
|  ⚠️   | The commit introduces a breaking feature. |
|  🆕,👋   | The commit introduces a non-breaking feature. |
|  🔀   | The commit merges two branches. |
| 🔀 ✅ | The commit resolves a merge conflict |
|  ⏪   | The commit reverts an existing change. |
|  ↗️   | The commit improves an existing feature or otherwise existing code. |
|  ♻️   | The commit removes unneeded or dead code. |
|  ✅   | The commit introduces one or more unit tests. |
|  🎨   | The commit introduces, modifies or removes assets such as images. |
|  🌐   | The commit introduces, modifies or removes localization such as translation files. |
|  📝   | The commit introduces documentation for code, instructions to compile, install or run code inside of the current repository. It may also be used for adding, changing or removing Markdown documents. |
|  ✏️   | The commit resolves a spelling mistake, such as a typo or grammatical error (within the changes of the commit, not the message itself). |
|  🚚   | The commit manages dependencies such as package.json files (adding, changing or removing). |
|  🚀   | The commit creates a new deployment. |
|  📦   | The commit version tags a deployment.|
|  🎉   | The initial commit. |

`[ Title ]` is a brief but descriptive title written in the imperative present tense. The `[ Title ]` must **not** end with a period as it is not a sentence, but a command. Each commit directs the repository to perform an action.

`[ Description ]` is optional text following the `[ Title ]`, which adds additional information about the changes the commit is introducing. It should only be included when the `[ Title ]` cannot fully describe the intent of the commit. The `[ Description ]` is typically included for critical or complex code, such as security patches.

The `[ Description ]` must begin with a new line to separate itself from the `[ Title ]`. This text should be grouped into small paragraphs, which are also separated by new lines. For improved context, links to external content or references are also encouraged to be included in the `[ Description ]`.


The `[ Title ]` and `[ Description ]` may also contain additional emojis to enhance the clarity and brevity of a commit message.

Example of a well formatted commit message: `🐛 Fix race condition introduced in 9e4d83a`

## Pro Tip

Sign your commits using your PGP key to verify you are the real author. Learn more about signed commits [here](https://help.github.com/articles/signing-commits-using-gpg).

