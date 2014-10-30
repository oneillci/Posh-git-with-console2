Posh-git-with-console2
======================

A reminder for the steps required for getting the posh git environment set up when installed via GH4W

1. Install GH4W - windows.github.com. This will install posh git but doesn't affect the global powershell env.
2. Install console2
3. Create C:\Users\{MY USERNAME}\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1 (create dir if not exists)
4. Paste the following:
  
  . (Resolve-Path "$env:LOCALAPPDATA\GitHub\shell.ps1")

  . $env:github_posh_git\profile.example.ps1


5. Ensure there is no startup dir specified in Console2 settings - this will allow GH4W to navigate to the repo directory
6. See http://haacked.com/archive/2012/05/21/introducing-github-for-windows.aspx/ and http://stackoverflow.com/questions/12504649/how-to-use-posh-git-that-comes-with-github-for-windows-from-custom-shell for more info
