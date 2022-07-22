## Git Configuration
```
git config --global user.name "User name"
git config --global user.email example@example.com
```
#### info regarding whole git config
```
man git-config
```

#### Set default editor
```
git config --global core.editor nvim
```
#### Set template for commit message
```
git config --global core.template <path-to-txt-file>
```
### Formatting and Whitespace
Formatting and whitespace issues are some of the more frustrating and subtle problems that many developers encounter when collaborating, especially cross-platform. It’s very easy for patches or other collaborated work to introduce subtle whitespace changes because editors silently introduce them, and if your files ever touch a Windows system, their line endings might be replaced. Git has a few configuration options to help with these issues.
```
core.autocrlf
```
If you’re programming on Windows and working with people who are not (or vice-versa), you’ll probably run into `line-ending issues` at some point. This is because Windows uses both a `carriage-return` character and a `linefeed` character for newlines in its files, whereas macOS and Linux systems use only the `linefeed character`. This is a subtle but incredibly annoying fact of cross-platform work; many editors on Windows silently replace existing LF-style line endings with CRLF, or insert both line-ending characters when the user hits the enter key.

Git can handle this by auto-converting `CRLF` line endings into `LF` when you add a file to the index, and vice versa when it checks out code onto your filesystem. You can turn on this functionality with the `core.autocrlf` setting. If you’re on a Windows machine, set it to true — this converts LF endings into CRLF when you check out code:
```
git config --global core.autocrlf true
```
