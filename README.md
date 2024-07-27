# AWS-Nuclei

## Description
AWS Cognito is a cloud-based identity and access management (IAM) service that provides functionality to add user registration and login features to web appliations and mobile application. AWS Cognito supports features such as multi-factor authentication, social identity providers (e.g., Facebook, Google), and user directory management. A common misconfiguration of the IAM service could allow an attacker to read sensitive Javascript files that have hardcoded IDs such as identityPoolId, userPoolWebClientId, and aws_cognito_identity_pool_id which can be used to gain unauthorized access to AWS services.

## Usage
`nuclei -u <url> -t aws-cognito-nuclei.yaml`

`katana -u <base url> -jsl -rl 50 | nuclei -t aws-cognito-nuclei.yaml`
