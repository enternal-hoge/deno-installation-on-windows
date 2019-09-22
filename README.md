# deno-installation-on-windows

Deno is a secure runtime for JavaScript and TypeScript built with V8, Rust, and Tokio.
https://github.com/denoland/deno

I tried to install and run deno on windows.

# Installation

## scoop

execute Power Shell administrator authority.

```
PS C:\Users\> Set-ExecutionPolicy RemoteSigned -Scope CurrentUser -Force
PS C:\Users\> iex (New-Object net.webclient).downloadstring('https://get.scoop.sh')
Initializing...
Downloading scoop...
Extracting...
Creating shim...
Downloading main bucket...
Extracting...
Adding ~\scoop\shims to your path.
'lastupdate' has been set to '2019-09-10T16:11:38.4105441+09:00'
Scoop was installed successfully!
Type 'scoop help' for instructions.
```

## deno

```
PS C:\Users\> scoop install deno
Installing 'deno' (0.17.0) [64bit]
deno_win_x64.zip (9.5 MB) [===================================================================================] 100%
Checking hash of deno_win_x64.zip ... ok.
Extracting deno_win_x64.zip ... done.
Linking ~\scoop\apps\deno\current => ~\scoop\apps\deno\0.17.0
Creating shim for 'deno'.
'deno' (0.17.0) was installed successfully!
```

## dinatra

dinatra is deno web framework, similar sinatra.

```
cd C:\Users\<CURRENT_USER>
git clone https://github.com/syumai/dinatra
cd dinatra\example
deno .\index.ts
deno run -A index.ts
```

access using browser.
http://localhost:8080/hello


