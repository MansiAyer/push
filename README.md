# push
*Automate changes and push to repo*
<hr>

Example usage:
```
steps:
- uses: MansiAyer/push@main
  with:
    script: update.py
    actions-token: ${{ secrets.GITHUB_TOKEN }}
```

<hr>

WIP | Goals:
* Accept python script, make changes, and push updates
* Parse input python script to check for dependencies and pip install requirements // does an action already exist for this?
* If no script input, then action must only attempt to push to remote
* Identify input script type, register ticket for each new type
* Expand existing to implement idenitifed script type, register ticket for unsupported types
