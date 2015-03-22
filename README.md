# Git Notes 

Sometimes there is things that you need to remember for development but there is no good way to remind you those things, without remember those places yourself.

```text
.git
├── branches
├── hooks
├── info
├── notes <
└── logs
```

This will add a place to place these notes, and then on commit it will show you those notes and have a confirm if there is notes there. So everythime you commit it will show you things you want to remember about your code. This will be branch specific and will be removed with the branch when deleted. 

## Example Usage

### commiting

```bash
git commit /cool-dir/noice.txt -m 'updating awesome stuff'
>
> Notes
> ==========
> Make sure to write awesome stuff
>
Hit Enter to Commit
```

### editing notes

```bash
git-notes
# opens up $editor for current branch notes
git-notes feature/specific-branch
```

### deleting note

```bash
git-notes remove
# remove current branch
git-notes feature/specific-branch
```