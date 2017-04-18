# CoreWebpack
April 2017

Simplest possible .NET Core app with MVC, Webpack, and TypeScript debugging. HMR (Hot Module Replacement) enabled in Webpack.

Features:
* F5 debugging of server code
* Auto refresh of TypeScript files (while running project, saving changes to TS files auto-updates the connected browser)
* TS sourcemapping. That is, adding 'debugger' to TS files correctly triggers TS files in browser F12 dev tools.

What it doesn't do:
* No auto refresh of cshtml pages. Must hit F5 in browser to see changes.
* TS breakpoints in VS will not be honored. Must debug using browser dev tools.

Notes:
* TS compiling done solely through webpack. Native compiling disabled by adding &lt;TypeScriptCompileBlocked&gt;true&lt;/TypeScriptCompileBlocked&gt; to csproj file and specifying an emtpy tsconfig.json file.
