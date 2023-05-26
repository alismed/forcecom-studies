## Suggestion Box

A project from [Trailhead Project](https://trailhead.salesforce.com/content/learn/projects/suggestion_box). Build a simple suggestion management app. No code required.

It is possible to use a [free trial environment](https://developer.salesforce.com/free-trials)
It is developed using the SFDX Cli, followed the steps bellow:
- Create the project
```bash
sfdx force:project:create -n suggestion-box
```
- Create a scratch box
```bash
sfdx force:org:create -s -f config/project-scratch-def.json -a BoxScratch
```

- Open the scratch box
```bash
sfdx force:org:open
```

- Create:
    - Custom objects and fields
    - Validation Rule
    - Record-Triggered Flow
    - Tab
    - Lightning App
    - Modify Page Layout
    - Global Action
    - Report
    - Dashboard
- Retrieve the components
```bash
sfdx force:source:pull
``` 
- Test your package in a new scratch org
```bash
sfdx force:org:create -s -f config/project-scratch-def.json -a BoxTestScratch
sfdx force:source:push -o BoxTestScratch
sfdx force:org:open -o BoxTestScratch
``` 

### Read All About It

- [Salesforce Extensions Documentation](https://developer.salesforce.com/tools/vscode/)
- [Salesforce CLI Setup Guide](https://developer.salesforce.com/docs/atlas.en-us.sfdx_setup.meta/sfdx_setup/sfdx_setup_intro.htm)
- [Salesforce DX Developer Guide](https://developer.salesforce.com/docs/atlas.en-us.sfdx_dev.meta/sfdx_dev/sfdx_dev_intro.htm)
- [Salesforce CLI Command Reference](https://developer.salesforce.com/docs/atlas.en-us.sfdx_cli_reference.meta/sfdx_cli_reference/cli_reference.htm)
