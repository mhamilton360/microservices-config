# microservices-config
Spring Cloud Config via Git

PS C:\Users\mhami> scoop
Usage: scoop <command> [<args>]

Available commands are listed below.

Type 'scoop help <command>' to get more help for a specific command.

Command    Summary
-------    -------
alias      Manage scoop aliases
bucket     Manage Scoop buckets
cache      Show or clear the download cache
cat        Show content of specified manifest.
checkup    Check for potential problems
cleanup    Cleanup apps by removing old versions
config     Get or set configuration values
create     Create a custom app manifest
depends    List dependencies for an app, in the order they'll be installed
download   Download apps in the cache folder and verify hashes
export     Exports installed apps, buckets (and optionally configs) in JSON format
help       Show help for a command
hold       Hold an app to disable updates
home       Opens the app homepage
import     Imports apps, buckets and configs from a Scoopfile in JSON format
info       Display information about an app
install    Install apps
list       List installed apps
prefix     Returns the path to the specified app
reset      Reset an app to resolve conflicts
search     Search available apps
shim       Manipulate Scoop shims
status     Show status and check for new app versions
unhold     Unhold an app to enable updates
uninstall  Uninstall an app
update     Update apps, or Scoop itself
virustotal Look for app's hash or url on virustotal.com
which      Locate a shim/executable (similar to 'which' on Linux)


PS C:\Users\mhami> scoop bucket add hookdeck https://github.com/hookdeck/scoop-hookdeck.git
Checking repo... OK
The hookdeck bucket was added successfully.
PS C:\Users\mhami> scoop install hookdeck
Installing '7zip' (23.01) [64bit] from main bucket
7z2301-x64.msi (1.8 MB) [===============================================================================================] 100%
Checking hash of 7z2301-x64.msi ... ok.
Extracting 7z2301-x64.msi ... done.
Linking ~\scoop\apps\7zip\current => ~\scoop\apps\7zip\23.01
Creating shim for '7z'.
Creating shim for '7zFM'.
Creating shim for '7zG'.
Creating shortcut for 7-Zip (7zFM.exe)
Persisting Codecs
Persisting Formats
Running post_install script...
'7zip' (23.01) was installed successfully!
Notes
-----
Add 7-Zip as a context menu option by running: "C:\Users\mhami\scoop\apps\7zip\current\install-context.reg"
Installing 'hookdeck' (0.8.5) [64bit] from hookdeck bucket
hookdeck_0.8.5_windows_amd64.tar.gz (3.7 MB) [==========================================================================] 100%
Checking hash of hookdeck_0.8.5_windows_amd64.tar.gz ... ok.
Extracting hookdeck_0.8.5_windows_amd64.tar.gz ... done.
Linking ~\scoop\apps\hookdeck\current => ~\scoop\apps\hookdeck\0.8.5
Creating shim for 'hookdeck'.
'hookdeck' (0.8.5) was installed successfully!
PS C:\Users\mhami> scoop bucket add hookdeck https://github.com/hookdeck/scoop-hookdeck-cli.git
WARN  The 'hookdeck' bucket already exists. To add this bucket again, first remove it by running 'scoop bucket rm hookdeck'.
PS C:\Users\mhami> scoop install hookdeck
WARN  'hookdeck' (0.8.5) is already installed.
Use 'scoop update hookdeck' to install a new version.
PS C:\Users\mhami> hookdeck login --cli-key 1gy3iqu4g4677o4k6jhdnloyh0cl09h54my3xcqfmj09stn66d
> Done! The Hookdeck CLI is configured with your console Sandbox
PS C:\Users\mhami> hookdeck listen 8071 Source
🚩 Not connected with any account. Creating a guest account...
? What path should the webhooks be forwarded to (ie: /webhooks)? /monitor
? What's your connection label (ie: My API)? localhost

Dashboard
👤 Console URL: https://api.hookdeck.com/signin/guest?token=3edyejqm3vj0lq5dgxmepnloq4qf2y608o23lkbbaj3njnhmzk
Sign up in the Console to make your webhook URL permanent.

Source Source
🔌 Webhook URL: https://hkdk.events/uKuCpYRVS1jQ

Connections
localhost forwarding to /monitor

> Ready! (^C to quit)
2023-12-21 23:35:23 [200] POST http://localhost:8071/monitor | https://console.hookdeck.com/?event_id=evt_Xrr4LAbW7jzOT23SOf
2023-12-21 23:39:56 [200] POST http://localhost:8071/monitor | https://console.hookdeck.com/?event_id=evt_GXdTraP5FeD9lTVlhR
2023-12-21 23:46:15 [200] POST http://localhost:8071/monitor | https://console.hookdeck.com/?event_id=evt_9HxhGlJ5htqdhisFYq
> Reconnected!
> Reconnected!
