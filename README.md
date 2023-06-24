# AspNetCoreConsoleStaticFiles
Shows how to serve static files through an ASP.NET core console application

The core is to set ".UseContentRoot(Directory.GetCurrentDirectory())" when setting up the host and "app.UseDefaultFiles()" and "app.UseStaticFiles()" when setting up the Startup class. Be sure to create a "wwwroot" subdirectory where it and its contents are copied to the output directory of the project (it cannot be served from the project folder, but from the output folder of the project).

And finally, you need to add the middleware for sharing static files. It's a nuget package and is called "Microsoft.AspNetCore.StaticFiles"
