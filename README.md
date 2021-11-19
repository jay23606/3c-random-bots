# 3c-random-bots
Creates random bots in 3c paper account as a way to see what settings and start conditions prevail

Instructions to run (linux):

dotnet new blazorserver --name random-bots

cd random-bots

dotnet add package XCommas

cp Index.razor /random-bots/Pages

dotnet run --urls=http://0.0.0.0:8080

Make sure port 8080 is available under firewall settings and navigate to page.

Run this in cloud instance to prevent hangup:

nohup dotnet run --urls=http://0.0.0.0:8080
