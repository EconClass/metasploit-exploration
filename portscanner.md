# The Port Scanner Modules

There are plenty of tools out there that let you scan for ports such as [`nmap`](https://nmap.org/download.html). However, Metasploit does come with its own module for port scanning, should you find yourself in a system that doesn't have one built in. Metasploit has a few types of port scanners available for us to use, so let's look at how to find them.

## First Steps

1. First we'll grab the ip address of the target machine by running the `ifconfig` command in the metasploitable machine which should look something like this:
![output](./assets/ifconfig.png)

2. Then, we're going to grab the `inet addr` from the second line of the output. In this case it's `192.168.0.33`. If you don't have a shared clipboard between your host and VM, or if you don't know what that means you can just jot it down somewhere and keep it handy.

3. Now, let's go back to our own computer, otherwise known as our host machine.

4. In our host machine's command line, run the command `msfconsole`. This will pull up something like this:
![msfconsole-start](./assets/msfconsole-start.png)
Don't worry if the ascii art isn't the same. They're generated randomly.

5. Next, we're going to search for the portscanner module by using the `search portscan` command in our msfconsole which looks like this:
![search-portscan](./assets/search-ps.png)

### TCP Port Scanner

The first scanner we are interested in is the `tcp` port scanner.
