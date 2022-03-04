# Synopsys CoPilot Gradle/GitHub CI Example

[![Actions](https://github.com/BlackDuckCoPilot/example-gradle-githubactions/workflows/Java%20CI/badge.svg)](https://github.com/BlackDuckCoPilot/example-gradle-githubactions/actions?workflow=Java+CI) [![Black Duck Security Risk](https://copilot-valid.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-gradle-githubactions/branches/validation/badge-risk.svg)](https://copilot-valid.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-gradle-githubactions/branches/validation)

Shows a working setup for using the Synopsys CoPilot integration to analyze the risk of project dependencies

## GitHub CI/CD Setup

The `.github/workflows/workflow.yml` file has been modified to upload dependency data to Synopsys CoPilot:

```yaml
- name: Upload to CoPilot
      run: bash <(curl -s https://copilot-valid.blackducksoftware.com/ci/githubactions/scripts/upload)
```
