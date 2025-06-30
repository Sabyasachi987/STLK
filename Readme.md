# stlk 🕵🏻‍♂️

<p align="center">
<img src="https://raw.githubusercontent.com/Sabyasachi987/STLK/master/assets/%40sabyasachi.png" alt="stlk logo" width="250" /></p>

A tiny Git-like version control system built with Node.js. 🚀  
Installable via npm, **stlk** mimics core Git functionality with a simplified design—perfect for learning or lightweight projects.


## 🚀 Installation

```bash
npm install -g stlk
```

## 🧠 Usage

```bash
stlk [options] [command]
```

### Global Options
| Option               | Description                   |
|----------------------|-------------------------------|
| `-V, --version`       | Output the version number     |
| `-h, --help`          | Display help information      |

## 🛠️ Commands

| Command                 | Description                                               |
|-------------------------|-----------------------------------------------------------|
| `init`                  | Initialize a new repository                                |
| `cat-file [options] <sha>` | Print the content of a blob by its SHA                   |
| `hash-object <file>`    | Hash and store a file as a Git object                     |
| `write-tree`            | Write the current index as a tree object                  |
| `checktree`             | Debug tree writing process                                |
| `commit-tree <args...>` | Create a commit from a tree                               |
| `log`                   | Show commit history                                       |
| `add <file>`            | Add a file to staging                                     |
| `unstage <file>`        | Unstage a file or all (with `.`)                          |
| `commit [options]`      | Commit staged changes                                     |
| `status`                | Show working tree status                                  |
| `branch [name]`         | List all branches or create one                           |
| `checkout <branch>` / `switch` | Switch to the specified branch                         |
| `merge [branch]`        | Merge a branch into the current one                       |
| `current-branch`        | Display the current branch                                |
| `diff <branchA> <branchB>` | Show diff between two branches                          |
| `help [command]`        | Get help for a specific command                           |

## 📦 Example Workflow

```bash
stlk init
stlk add index.js
stlk commit -m "Initial commit"
stlk log
stlk branch feature
stlk switch feature
stlk diff main feature
```

## 📁 Project Structure

All internal objects are stored in the `.stlk` directory, similar to Git’s `.git` folder:

```perl
.stlk/
├── objects/
├── refs/
├── HEAD
└── index
```

## 📚 Learning Purpose

This tool is built to understand how Git works under the hood — exploring blobs, trees, commits, and branching without the full complexity of Git internals. 

## ✨ Credits

Developed by [@sabyasachi987](https://github.com/sabyasachi987)

## 📜 License

ISC  
© 2025 Sabyasachi — Sole developer and owner of the stlk project