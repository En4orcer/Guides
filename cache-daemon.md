## Cache Daemon Guide

**Table of contents:**
- [Public Node](https://github.com/Cache-core/Guides/blob/master/cache-daemon.md#public-node)
- [Local Node](https://github.com/Cache-core/Guides/blob/master/cache-daemon.md#local-node)
- [Useful Daemon Commands](https://github.com/Cache-core/Guides/blob/master/cache-daemon.md#useful-daemon-commands)

***

#### Public Node

Public Nodes help decentralise the network because more independant people are connecting to the Blockchain rather than a centralised source.
Public Nodes are also used to help people in a different geo-location get a better connection with the Blockchain itself.
Read about [Ping](https://en.wikipedia.org/wiki/Ping_(networking_utility)) to learn why this would be an advantage if more people have better ping across the network.

There are incentives for people running public nodes with the built-in features it has to offer.
With 2 commands, you can set your node up to charge a fee whenever someone using your node wishes to make a transaction.
The 2 commands are:
```
--fee-address=<address>
--fee-amount=<amountInAtomicUnits>
```

`--fee-address` can be set to your primary wallet address.
You cannot use integrated addresses when using this feature!
We use atomic units to calculate the node fee which means instead of typing `--fee-amount=1.23456`, you would type `--fee-amount=123456`.
That being said, there is a cap on how much a node operator can charge p/transaction so people are not over-charged when using these public services run by 3rd parties.
The current cap is `1.00000 $CXCHE`, 1 full unit of the coin which is `100000` in atomic units.

> [Note] A common error when setting up a public node is a FIREWALL issue.
> Please make sure your ports are open so external machines can read the data you're trying to provide

##### Linux & MacOS Terminal

Open your terminal where your Cache binaries are located and follow the below example:

```bash
$ ./cache-daemon --bind-rpc-port <port>
```

Find your machines IP address and then open a browser and goto `http://<ip>:<port>/getInfo`.
If there is information displayed, then your node is successully public.

##### Windows .bat Contents

As stated above, you need to launch the programs via a `.bat` file rather than the standard double-click way that most other programs are launched.
This should be the contents of your `.bat` file:

```bash
cache-daemon.exe --bind-rpc-port=<port>
pause
```

Find your machines IP address and then open a browser and goto `http://<ip>:<port>/getInfo`.
If there is information displayed, then your node is successully public.

***

#### Local Node

A local node is a node that does not feed the network with information about the Blockchain.
It is confined to your machine and the network seeds to obtain the correct Blockchain information.

Launching a Cache Daemon is simple, even if you're setting up a [Public Node]().
The examples shown here are for Linux, MacOS and Windows.

> [Note] When using Windows, you need to launch the client software via a `.bat` file and not by double-clicking or the programs will fail to load.

##### Linux & MacOS Terminal

Open your terminal where your Cache binaries are located and follow the below example:

```bash
$ ./cache-daemon
```

That's how simple it really is.
Just loading the program with no added flags is enough for your local node to gain the information directly from the Blockchain.

##### Windows .bat Contents

As stated above, you need to launch the programs via a `.bat` file rather than the standard double-click way that most other programs are launched.
This should be the contents of your `.bat` file:

```bash
cache-daemon.exe
pause
```

That's how simple it really is.
Just loading the program with no added flags is enough for your local node to gain the information directly from the Blockchain.

> [Note] We use a `pause` command within the `.bat` file just in case the cache-daemon fails to load.
> It will pause `cmd` so you're able to clearly see the error.

***

#### Useful Daemon Commands

- `status`
  - Displays information about your daemon and the blockchain.
- `ban <ip> <seconds>`, `unban <ip>` & `print_ban`
  - Used if a node is causing your node to misbehave, usually syncing problems.
- `start_mining <address> <threads>`, `stop_mining`, `show_hr` & `hide_hr`
  - Used to solo-mine the network using your CPU.
- `print_cn` & `print_pl`
  - Displays the current connections and peer list.

