Aim :
	ASP.NET Core SignalR with TypeScript and Webpack

Reference Link :
	https://docs.microsoft.com/en-us/aspnet/core/tutorials/signalr-typescript-webpack?view=aspnetcore-2.2&tabs=visual-studio-code
	
Step:
1) Create folder SignalRWebPack.. -->  project root
2) Open console open specific location  
	dotnet new web -o SignalRWebPack 	
	npm init -y  --> it will create package.json
3) Open  package.json
	 add  "private": true,
4) execute command in command prompt
	npm install -D -E clean-webpack-plugin@1.0.1 css-loader@2.1.0 html-webpack-plugin@4.0.0-beta.5 mini-css-extract-plugin@0.5.0 ts-loader@5.3.3 typescript@3.3.3 webpack@4.29.3 webpack-cli@3.2.3
5) Open  package.json 
	"scripts": {
	  "build": "webpack --mode=development --watch",
	  "release": "webpack --mode=production",
	  "publish": "npm run release && dotnet publish -c Release"
	},	
6) Create a file named webpack.config.js
	refer reference link 
7) Open console with location
	npm run release
	dotnet run
8) Open SignalRWebPack cs project (Execute)