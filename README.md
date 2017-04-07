# ubik
Quickly spin up/down and SSH to/from a locally hosted VirtualBox server. Safe when taken as directed.

Inspired by PKD's [book of the same name](https://en.wikipedia.org/wiki/Ubik), this script seamlessly transports the user between machines, starting and stopping as necessary. The goal is to not have to think about names, ports, &c., when making the shift: it should be as easy to operate as an aerosol can. It's therefore designed to have parameters in the script itself rather than passed via command-line.

Assumptions made:
- Running Cygywin on Windows, or something else that has access to the Windows host's VBoxManage command *and* a working command-line SSH executable
- Running VirtualBox on Windows host, running Linux VM on VirtualBox as guest, with NAT and port forwarding enabled.

Recommended:
- Set up SSH key authentication to avoid password prompts!

For a more detailed write-up, see the blog post: http://corysalveson.com/post/headless-with-ubik/
