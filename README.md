# PowerRemoteShell
A Powershell App to run Powershell code or scriptblock on multiple remote hosts simultaneously.

Read more at https://powershellchronicles.com/portfolio/power-remote-shell/

# Why do you want to use PowerRemoteShell?
1. Do you often find yourself writing scripts to execute a piece of powershell or cmd code on multiple remote machines?
2. Do you often use/wish to use multithreading just so you could have it run in parallel rather than in series?
3. How would you like to have a platform that will take care of that hurdle for you?

If you answered 'Yes' to any of those questions, that is why you should use PowerRemoteShell.

![alt text](https://github.com/RohinSidharth/PowerRemoteShell/blob/master/ScreenShot/PowerRemoteShell.jpg)

# Under The Hood
This is nothing fancy. It is just a GUI wrapper written in Sapien PowerShell Studio that does the looping and multithreading for you.
It uses Invoke-Command and Psexec [Redundancy in case WinRM is not configured/faulty] to execute your scriptblock LOCALLY on the target machines.

# How to Use
1. Add remote hosts list on the left panel using the 'Add Host' button.
2. Insert your scriptblock or command [Powershell, Native CMD, Multiline scripts] on the scriptblock box on top panel
3. Hit Execute
4. Wait for it to finish executing. the process is parallel
5. When finished, click on individual hosts to view its corresponding results on the right side panel.

Recommend reading more at https://powershellchronicles.com/portfolio/power-remote-shell/
