## Known Environment Issues
- When creating or pushing PRs with `gh` CLI and TLS certificate errors occur, immediately use `--no-verify` for git push or the appropriate insecure flag for `gh`. Do not suggest macOS keychain debugging or other root-cause investigations unless explicitly asked.

## Code References
- When referencing code (explaining, discussing, or pointing to specific logic), always use clickable Markdown links with the fully qualified file path and line numbers
- Format: `[file.go:42](file:///full/path/to/file.go:42)` or `[file.go:42-50](file:///full/path/to/file.go:42)` for ranges
- Never use relative paths or omit line numbers when referring to specific code
- Always use `file://` URI scheme so links are clickable in the terminal/IDE

## Give feedback
- If you find any of my instructions too verbose/not clear enough/have gaps/mislead you, dump your feedback in .local/aifeedback and let me know. Give clear examples so that I can improve

## When Asked To Plan
- Look for `.local/aitasks` directory
- Create task folder: `/<YYYY-MM-DD>/<task-name>/`
- Always create `plan.md` with the implementation plan
- Create additional files as needed:
  - `checklist.md` - Work items with ✅/⬜ status
  - `notes.md` - Research, discoveries, scratch pad
  - `deliverables.md` - What was shipped (PRs, files changed)
  - `feedback.md` - Post-mortem, what worked/didn't
  - `context/` - Subfolder for reference files (specs, screenshots, code dumps)
- Don't code anything outside of the plan doc. Consult the user before executing the plan

### Task Status
Track status at the top of `plan.md`:
```
Status: in-progress | blocked | completed | abandoned
```

### Plan Style Guide
- Break down plans into clear sections with headings
- Break down implementation steps into phases
- Add examples and code snippets in each implementation phase

## Shorthand Communications
All of the following shorthand communications should be strictly applied to the immediate conversation it was mentioned. They should not be applied to any of the subsequent conversations unless they are explicitly mentioned again

- "airec" means "don't make any changes yet, just give me your recommendations"
- "aiask" means "do what i just asked but consult me before taking the next step"
- "aiexp" means "don't make any changes, just explain to me"
- "aiplan" means "create a plan in .local/aitasks. consult me before coding"
- "ainobk" means "don't worry about backward compatibility"
- "aitt" means "use table driven style. use SetupTest, SetupSubTest, TearDownSubTest, TearDownTest. aiflw"
- "aiprt" means "compare the current branch with main and suggest the proper PR title. follow the PR template in the repo (.github/pull_request_template.md) for the PR body. aishort"
- "aipr" means "if in master/main, switch to a new branch. create a PR from the branch. aiprt. PR description must be written for reviewers, no conversation summaries."
- "aiprd" means "aipr but create in draft mode"
- "aiprr" means "there's already an existing PR. update it"
- "aiflw" means "follow other examples in this repository"
- "aixbox" means "don't be limited by what I said, think freely"
- "aishort" means "be short and to the point"
- "airej" means "feel free to say no"
- "aieval" means "evaluate the statement above and let me know what you think. don't make any changes"
- "ainote" means "jot down notes of our conversation in ./local/ainotes. update the notes after each back and forth. write notes in .md and organize by discussion topic"
- "aisub" means "use a sub-agent to do what i said"

If I typed something like "aixxx" that you don't understand, ask
