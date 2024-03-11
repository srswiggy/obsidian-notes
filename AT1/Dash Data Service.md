- Get AWS CLI and get Shuttle (through the Doc)
- Remove the Aws CaUsername (everything including the ternany operator)
- Login to Shuttle SSO `aws sso login --profile shuttlesso`
- after that export the credentials of aws
```
export JAVA_ARTIFACTORY_READ_ENDPOINT=[https://swiggy-domain-157529275398.d.codeartifact.ap-southeast-1.amazonaws.com/maven/swiggy-java-repository](https://swiggy-domain-157529275398.d.codeartifact.ap-southeast-1.amazonaws.com/maven/swiggy-java-repository) 
export JAVA_ARTIFACTORY_READ_USERNAME=aws 
export JAVA_ARTIFACTORY_READ_PASSWORD=`aws codeartifact get-authorization-token --domain swiggy-domain --domain-owner 157529275398 --region ap-southeast-1 --query authorizationToken --output text --profile shuttlesso`
```
- restart the ide
- 