# 3c-random-bots
Creates random bots in 3c paper account as a way to see what settings and start conditions prevail (my first blazor project)

Instructions to run (linux):

Install .net sdk https://docs.microsoft.com/en-us/dotnet/core/install/

dotnet new blazorserver --name random-bots

cd random-bots

dotnet add package XCommas.Net

cp Index.razor /random-bots/Pages

dotnet run --urls=http://0.0.0.0:8080

Make sure port 8080 is available under firewall settings and navigate to page.

Run this in cloud instance to prevent hangup:

nohup dotnet run --urls=http://0.0.0.0:8080

To kill it later:

ps -ef
kill <pid> 
