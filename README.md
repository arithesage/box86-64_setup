# [WIP] Box86-64 Setup

For easily setup both Box86 and Box64.

Box86 is a program that allows executing 32 bits x86 applications in a
ARM system, and Box64 do the same, but for 64 bits applications.

The main scripts here are 'setup-proot' for setting up Box86-64 in a
Termux proot container and 'setup-distrobox' for setting it up in a
docker/podman container using distrobox (mainly for testing purposes).


The rest of scripts are:

- bexec: Execute a command line in container with Box86-64.
- bexec_admin: Same as 'bexec' but with root privileges.
- box86-installer: Installs Box86.
- box64-installer: Installs Box64.
- boxenter: Enters a container.
- boxenter_admin: Same but with root user.

- boxify: Creates an script for running a x86/x86_64 program with
          Box86-64. The script uses the program original filename and
          the real executable is renamed adding '_x86'.

- setup-box86: Setups Box86 in a container.
- setup-box64: Setups Box64 in a container.

- unboxify: Revert the changes made by boxify
