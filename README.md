# taskfiles
Shared tasks to streamline workflow.

## Usage
Reference the listed task config files in your local `Taskfile.yml` using `includes`.

    ```yaml
    version: '3'

    includes:
      tf:
        taskfile: https://github.com/jkim-mlops/taskfiles.git/terraform.yml?ref=0.1.0
        dir: deployment

    tasks:
      deploy:
        cmds:
          - task tf:apply
    ```
