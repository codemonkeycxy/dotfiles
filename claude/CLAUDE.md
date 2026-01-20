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
- "aiprt" means "compare the current branch with main and suggest the proper PR title and a 'why' seciton. aishort"
- "aipr" means "create a PR from the current branch. aiprt"
- "aiflw" means "follow other examples in this repository"
- "aixbox" means "don't be limited by what I said, think freely"
- "aishort" means "be short and to the point"
- "airej" means "feel free to say no"
- "aieval" means "evaluate the statement above and let me know what you think. don't make any changes"
- "ainote" means "jot down notes of our conversation in ./local/ainotes. update the notes after each back and forth. write notes in .md and organize by discussion topic"

If I typed something like "aixxx" that you don't understand, ask