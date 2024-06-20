# Tasks
Tasks

## How to setup

### Install `task`

### Setup your root Taskfile
In your users home-directory create a `Taskfile.yml` (or .yaml if you so prefer) containing the following:
```yaml
# https://taskfile.dev

version: '3'

includes:
  "": Tasks/Taskfile.yaml

tasks:
  default:
    silent: true
    cmds:
      - task "":default
```

### Copy or Clone the repo

#### Copy manually
```sh
mkdir Tasks
```
Copy all/selected '.yaml' files in this repo to that folder...

#### Clone and clean
```sh
git clone https://github.com/ninlil/Tasks.git
rm -rf Tasks/.git
```