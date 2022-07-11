# Black Duck CoPilot Gradle/GitHub CI Example

[![Actions](https://github.com/BlackDuckCoPilot/example-gradle-githubactions/workflows/Java%20CI/badge.svg)](https://github.com/BlackDuckCoPilot/example-gradle-githubactions/actions?workflow=Java+CI) |[![Security Risk - CoPilot](https://copilot-test.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-gradle-githubactions/branches/test/badge-risk.svg)](https://copilot-test.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-gradle-githubactions)|

Shows a working setup for using Synopsys CoPilot to analyze the risk of project dependencies

## GitHub CI/CD Setup

The `.github/workflows/workflow.yml` file has been modified to upload generated dependency data to Black Duck CoPilot:

```yaml
- name: Upload to CoPilot
      run: bash <(curl -s https://copilot-test.blackducksoftware.com/ci/githubactions/scripts/upload)
```
