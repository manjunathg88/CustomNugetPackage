# CustomNugetPackage

This project contains a yaml file that has the script to create the Azure ci pipeline which creates a custom Nuget package

Instructions:
1. Login to Azure DevOps
2. Navigate to the Pipelines hub.
3. Click New Pipeline. We will use the wizard to automatically create the YAML definition based on our project.
4. Select the Azure Repos Git as the source hosting platform. Note the others supported.
5. Select the CustomNugetPackage repo.
6. Select the ASP.NET template as the starting point for your pipeline.
7. Review the contents of the YAML definition. It will be saved as a new file called “azure-pipelines.yml” in the root of the repository and contain everything needed to build and test a typical ASP.NET solution. You can also customize the build as needed. In this case, update the pool to specify the build should use a Visual Studio 2017 build VM.
8. Review trigger and point to master if you repo does not have main (new repos will have “main” instead of “master”).
9. Click Save and run.
10. Click Save and run to confirm the commit.
11. Track the build until it is completed. Click Job to see the logs.
12. Each task from the YAML file is available for review, including any warnings and errors.

More details on: https://azuredevopslabs.com/labs/azuredevops/yaml/
