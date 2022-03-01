Some Common troubleshooting
----------------------------------------------------------------------------------------------
1. Not enough space in /var/cache/apt/archives 

You will encounter this issue when downloading packages from any repository
For me when i was downloading Docker inside my vm
by -> `apt install docker.io` then this packages was not finding enough free space in the directory 

As root was mounted on "/" , i saw the disk usage by
- `sudo du -sh /var/cache/apt/archives `

It was 100% utilised and now i removed one file which was 500GB and ran again the same command and now the docker was install successfully

Also just try below commands

- `sudo apt clean`

The clean command clears out the local repository of downloaded package files. It removes everything except the partials folder and lock file from /var/cache/apt/archives/.

- `sudo apt autoremove`

The autoremove option removes packages that were automatically installed because some other package required them but, with those other packages removed, they are no longer needed. Sometimes, an upgrade will suggest that you run this command.

- `apt-get autoclean`

The apt-get autoclean option, like apt-get clean, clears the local repository of retrieved package files, but it only removes files that can no longer be downloaded and are virtually useless. It helps to keep your cache from growing too large.