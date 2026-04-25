*This project was created by khaled as part of the OnRampAcademy AI Enhanced Senior Track*

## Description

This project is our gateway into learning Github Actions and pull request and how the workflow works to better know how to manage git better and gain experience.

workflow files have .yml extension
syntax:
name: workflow name shown in Actions tab
on: what triggers it
jobs: what work runs
runs-on: machine type
steps: commands to execute
Nesting matters since yaml is indentation-sensitive
on
  workflow_dispatch
    inputs
      name
For yaml files, use 2 spaces to avoid bugs
One workflow must be manually triggered
the other must automatically run when code is pushed to main
Github treats a merge into main as a push event to branch main
to make it trigger on main pushes do
on: push: branches: -main
runs-on: Running our workflow on a github provided Ubuntu vm.
