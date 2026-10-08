# Architecture

## Structure
```
.
├── .editorconfig             # EditorConfig: UTF-8, LF, final newline; Markdown 2-space indent
├── .markdownlint-cli2.yaml   # markdownlint-cli2 config (default rules, MD013 off)
├── LICENSE     # MIT license
└── README.md   # describes the repo's purpose (branch-protection / bot-review test)
```

The repository has no application code, modules, entry points or data flow. It only serves as a target for pull requests and reviews, used to see whether a Coditor bot review satisfies GitHub's required-approvals branch protection rule.
