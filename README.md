# Introduction

This is a template for using dotnetcore 3.1 with aws lambda functions

## Using the Template

### Template installation

To install the template :

- Clone the project locally
- In the root folder run

```sh
dotnet new -i .\
```

After running that, you now have access to a template with a short name of `serverless.DotNetCore3`

To uninstall the Template

```sh
dotnet new -u <ABSOLUTE_FILE_SYSTEM_DIRECTORY>
```

### Template usage

Once installed you can now create a new project based on the template.

Navigate to a folder where you want to create the project in.

```sh
dotnet new serverless.DotNetCore3 -sn {function name}
```

for example

```sh
dotnet new serverless.DotNetCore3 -sn sample
```

This will create a solution and function project for you, including a sample controller and sample unit test

## Local testing

You can test it locally by debugging with the IIS Express option.

For the default project that starts up with the template, navigate to

```sh
localhost:{PORT}/api/values
```

## Lambda deployment

To deploy the function to AWS

```sh
dotnet lambda deploy-serverless
```

And follow the standard process as recommended by AWS
