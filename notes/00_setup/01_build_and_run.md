1. Build the project using 

``` 
dotnet build 

# dotnet build "/path/to/proj.csproj" 
```


2. Run the project using

``` 
dotnet run

# dotnet run --project "path/to/proj.csproj --launch-profile https
```

or if you need hot-reloading

```
dotnet watch run
```

**Note** 
- From dotnet core 7 onwards, http and https profile has been split, and by default, it will launch the first profile it finds. So if you want https, either edit launchSettings.json and move https on top of profile list, or use `--launch-profile https` as launch parameter. 
*https://github.com/dotnet/aspnetcore/pull/42027, https://github.com/dotnet/sdk/issues/29569#issuecomment-1416109409*

**Note:**
- When you `watch` the project, it will create a websocket to the client.
- Sometimes you might end up with issues related to watching, in that case, rebuild the project by running without watch, then close it and run watch command again.
