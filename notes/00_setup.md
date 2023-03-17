We install dotnet core and its command line tool for your operating system.

We then create a new razor project with following command
```
dotnet new razor -o CrudApp
```

By default, it does not create a solution file, but since most editors still use it, it is better to have it. We can generate it using following command.

``` 
dotnet new sln
```

then we add current project into the sln using 

``` 
dotnet sln add .
```

This command will register the `.csproj` file into the `.sln` file. 



**Note:**
- Recommended extensions for vs-code/code-oss is "C# with omnisharp" and  "vscode-solution-explorer"
- "vscode-solution-explorer" can conflict with the solution file generated with commands above. If this happens then delete the sln file and use the extension to generate a new sln file and add the project to it, This will create using more explicit commands that should reduce chances for id conflicts to happen. 
