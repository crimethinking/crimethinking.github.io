# Use classic Windows theme for login/logoff UI
The switchover from Luna theme to classic in XP is jarring. To make XP login/logoff UI
looking like that of Server 2003, [use the `at.exe` trick and set the `SYSTEM` account
theme to classic](http://wp.xin.at/archives/5621). Massive shoutout to Thrawn

* Launch a `cmd` with admin rights, run `at.exe <time + 1 minute> /interactive "cmd.exe"`
to launch another `cmd` with `SYSTEM` privileges
* Kill `explorer.exe` using Task Manager
* Use the `SYSTEM` CLI to spawn an `explorer.exe` shell
* Set whatever visual settings you want to. I use classic
* Logoff

!!! failure "[Tweak UI method](http://wp.xin.at/archives/5621#comment-173806)"
    Did not work. Copying user settings over to `SYSTEM` with Tweak UI created
    a mishmash of Luna and classic that was even more jarring