# Week 0 — Billing and Architecture

# Install AWS CLI
* We are going to install the AWS CLI when our Gitpod enviroment lanuches.
* We are are going to set AWS CLI to use partial autoprompt mode to make it easier to debug CLI commands.
* The bash commands we are using are the same as the [AWS CLI Install Instructions]https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html

# Configure AWS CLI Auto-Prompt
The AWS CLI provides an auto-prompt feature that guides you interactively through commands and options, making it easier to use the CLI efficiently.
 Use the command: 
* Enable Auto-Prompt Mode:
        You can enable auto-prompt mode in two ways: session-specific and persistent configuration.

  *Enable Auto-Prompt for a Single Session

To enable auto-prompt mode for your current session, use the command:
 `aws --cli-auto-prompt `

  * Enable Auto-Prompt Persistently

To enable auto-prompt mode persistently across all sessions, you need to update the AWS CLI configuration file.
 Open or create the config file in the .aws directory:

 `vi ~/.aws/config`

Add the following line under the [default] section: 
`ini
[default]
cli_auto_prompt = on `

This will persist the cli auto-prompt