We install dotnet core and its command line tool for your operating system.

We then create a new razor project with following command

```
dotnet new razor -o CrudApp
```

By default, it does not create a solution file, but since most editors still use it, it is better to have it. We can generate it using following command.

``` 
dotnet new sln

# dotnet new sln -n "project_name"
```

then we add current project into the sln using 

``` 
dotnet sln add .

# dotnet sln "path/to/proj.sln" add "/path/to/proj.csproj"
```

This command will register the `.csproj` file into the `.sln` file. 
