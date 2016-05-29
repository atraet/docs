# ASP.NET Core 1.0 Fundamentals

## 2. Startup and Middleware

2 default middlewares
- IISPlatformHandler (authorization)

Terminal middleware: no next

```cs
app.UseWelcomePage();
app.UseRuntimeInfoPage();

```

*Order of the middlewares is important.*

Workflow to use middlewares
- install middleware (NuGet Package)
- register middleware in Startup.Configure().

### Middleware which matches environment variables
Project -> Properties -> Debug

### Serving Files
- serving static Files
- default files

### Setting up ASP.NET MVC middleware
3 steps to set up ASP.NET MVC
- add package dependency
- add MVC service
- add MVC middleware

## 3. Controllers in the MVC Framework
### Routing
2 ways to specify routes
- conventional routes
- attribute routes
