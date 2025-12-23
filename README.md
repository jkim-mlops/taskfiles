# taskfiles
Shared tasks to streamline workflow.

## Usage
1. Clone this repository to your local `$HOME` directory. I've cloned it into my `projects` folder subdirectory.

1. Create a `Taskfile.yml` file in your `$HOME` directory with

```yml
version: '3'

includes:
  tf:
    taskfile: ./projects/taskfiles/terraform.yml

tasks:
  default:
    cmds:
      - task --list
```

1. Globally reference the tasks with the `-g` flag.

    ```
    task -g
    ```
