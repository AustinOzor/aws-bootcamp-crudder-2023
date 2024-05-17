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
`ini `
`[default]`
`cli_auto_prompt = on`

This will persist the cli auto-prompt

# Create a new User and Generate AWS Credentials
 Login to aws console with your account details
* Enable console access for the user
* Create a new Admin Group and apply AdministratorAccess
* Create the user and go find and click into the user
* Click on Security Credentials and Create Access Key
* Choose AWS CLI Access
* Download the CSV with the credentials
  
  ![week0 iam user](https://github.com/AustinOzor/aws-bootcamp-crudder-2023/assets/99667583/e9d6dce3-1ef0-4a9e-a8e8-96f0d619e150)

# Set Environmental Variables:
`export AWS_ACCESS_KEY_ID="" `
`export AWS_SECRET_ACCESS_KEY="" `
`export AWS_DEFAULT_REGION=us-east-1`

![ENV VAR](https://github.com/AustinOzor/aws-bootcamp-crudder-2023/assets/99667583/cbbdd739-159d-4786-a714-c289cf8ca042)
