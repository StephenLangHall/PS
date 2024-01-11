# PS: Project Save Script

PS saves projects into the '...' directory in this file structure:

```
.../
  Version
  Saves/
    <version>.zip
  Diffs/
    <last-version>:<next-version>.diff
  Last/
    <last revision>
```

# Arguments

`PS init <remote-save-directory>` to start a project, the remote location is optional. It should be in the format "user@host:/save/directory/"

`PS save` to save a project: this will create the following files:
```
  .../Saves/<version>.zip
  .../Diffs/<last-version>.diff
```

`PS push` to update the backup at remote save location
