## Cache Wallet Guide

**Table of contents:**
- [Wallet Options]()
  - [Create Wallet]()
  - [Import Wallet]()
    - [Import with Seed]()
    - [Import with Secret Keys]()
  - [Open Wallet]()
- [Node Connection]()
  - [Local Node Connection]()
  - [Remote Node Conncection]()
- [Transfer]()
- [Backup Wallet]()

> We show the private keys of an empty wallet here. Please never share them with anyone else, this is done as an example for the expected output.

***

#### Wallet Options

There are 3 ways to obtain your wallet using the Cache client wallet.
Creation of a new wallet, importing the keys of an old wallet or opening a wallet thats already been created/restored locally.
Whichever one you choose, using the `cache-wallet` is the most secured way to use your wallet as no 3rd parties are involved.

***

##### Create Wallet

Upon loading `cache-wallet`, you are prompted with an option on what to do:

```
Welcome, please choose an option below:

        [G] - Generate a new wallet address
        [O] - Open a wallet already on your system
        [S] - Regenerate your wallet using a seed phrase of words
        [I] - Import your wallet using a View Key and Spend Key

or, press CTRL_C to exit: 
```

In this instance, we want to create a wallet so go ahead and type **G** then press enter.

Now, you'll need to type a new wallet name and then create and confirm a password (this can be left blank if you don't share your local machine).

```
Specify wallet file name (e.g., name.wallet).
What do you want to call your new wallet?: myFirstCacheWallet
Give your new wallet a password: 
Confirm your new password: 
Wallet Address: cxcheA7uHhRFGn8V2nNUMgW9xuVaxwjTmhXUu2mcTCXCZZcdUgyePU1g5yXkzRh76dEB5J9ShBvmCAXNcWt5oNzweuK8yfKy5k5
Private spend key: c06b651bafe22a7172410f44615922ee3bee2be9190137340d6f97f63100a309
Private view key: 1a482f111ed040116ed85ef15b9933e776158d8bb15a64486333c4bbe9bddd00
Mnemonic Seed: eavesdrop avoid deepest smash uptight guarded assorted wallets duets bifocals eccentric colony talent kiwi hiding puffin agenda dwindling video romance quick nibs riots segments guarded
**********************************************************************
Your wallet has been generated.
```

If the wallet was successful in creating a new wallet, you should see something similar to the above example.
In the example we used **myFirstCacheWallet** as the wallet name.
As you can see, your wallet information is displayed so you can copy & paste this to a safer place and to login to your new wallet.

**BE AWARE**
`Private spend key:` & `Mnemonic Seed:` should never be shared to another person as these are the vital login details for your wallet.
`Private view key:` can be used for view-only wallets.

***

##### Import Wallet

Upon loading `cache-wallet`, you are prompted with an option on what to do:

```
Welcome, please choose an option below:

        [G] - Generate a new wallet address
        [O] - Open a wallet already on your system
        [S] - Regenerate your wallet using a seed phrase of words
        [I] - Import your wallet using a View Key and Spend Key

or, press CTRL_C to exit: 
```

Depending how we want to import our wallet, we will either choose **S** or **I**.

###### S - Import using Seed Phrase

In this instance, we want to import our wallet using the seed phrase so go ahead and type **S** then press enter.

Now, you'll need to type a new wallet name and then create and confirm a password (this can be left blank if you don't share your local machine) and provide the wallet with the seed phrase.

```
Specify wallet file name (e.g., name.wallet).
What do you want to call your new wallet?: myFirstCacheWallet
Give your new wallet a password: 
Confirm your new password: 
Mnemonics Phrase (25 words): eavesdrop avoid deepest smash uptight guarded assorted wallets duets bifocals eccentric colony talent kiwi hiding puffin agenda dwindling video romance quick nibs riots segments guarded
Imported wallet: cxcheA7uHhRFGn8V2nNUMgW9xuVaxwjTmhXUu2mcTCXCZZcdUgyePU1g5yXkzRh76dEB5J9ShBvmCAXNcWt5oNzweuK8yfKy5k5
**********************************************************************
Your wallet has been imported.
```

If the wallet was successful in importing a new wallet, you should see something similar to the above example.

###### I - Import using View & Spend Key

In this instance, we want to import our wallet using the secret keys so go ahead and type **I** then press enter.

Now, you'll need to type a new wallet name and then create and confirm a password (this can be left blank if you don't share your local machine) and provide the wallet with the secret keys.

```
Specify wallet file name (e.g., name.wallet).
What do you want to call your new wallet?: myFirstCacheWallet
Give your new wallet a password: 
Confirm your new password: 
Private Spend Key: c06b651bafe22a7172410f44615922ee3bee2be9190137340d6f97f63100a309
Private View Key: 1a482f111ed040116ed85ef15b9933e776158d8bb15a64486333c4bbe9bddd00
Imported wallet: cxcheA7uHhRFGn8V2nNUMgW9xuVaxwjTmhXUu2mcTCXCZZcdUgyePU1g5yXkzRh76dEB5J9ShBvmCAXNcWt5oNzweuK8yfKy5k5
**********************************************************************
Your wallet has been imported.
```

If the wallet was successful in importing a new wallet, you should see something similar to the above example.

***

##### Open Wallet

Upon loading `cache-wallet`, you are prompted with an option on what to do:

```
Welcome, please choose an option below:

        [G] - Generate a new wallet address
        [O] - Open a wallet already on your system
        [S] - Regenerate your wallet using a seed phrase of words
        [I] - Import your wallet using a View Key and Spend Key

or, press CTRL_C to exit: 
```

In this instance, we want to open a wallet so go ahead and type **O** then press enter.

```
Specify wallet file name (e.g., name.wallet).
Enter the name of the wallet you wish to open: myFirstCacheWallet
Enter password: 
Loading wallet...
Loaded 0 known transfer(s)
Opened wallet: cxcheA7uHhRFGn8V2nNUMgW9xuVaxwjTmhXUu2mcTCXCZZcdUgyePU1g5yXkzRh76dEB5J9ShBvmCAXNcWt5oNzweuK8yfKy5k5
```

If the wallet was successful in opening your wallet, you should see something similar to the above example.

***

#### Node Connection

You have two options when it comes to connection `cache-wallet` to a daemon. You can either:
a) Connect the wallet to your local node
b) Connect the wallet to a remote node
When connecting to a remote node, you could be paying a service charge to that node when you send a transaction. (Max Fee has been capped to 1 $CXCHE p/Transaction to avoid people taking advantage of this)

***

##### Local Node Conncection

To connect to a local node, you must first have an instance of `cache-daemon` running and fully synced with the blockchian.
You can use [this guide for the Cache Daemon](https://github.com/Cache-core/Guides/blob/master/cache-daemon.md#local-node) to learn how to setup a local node.

> [Note] When using Windows, you need to launch the client software via a `.bat` file and not by double-clicking or the programs will fail to load.

###### Linux & MacOS Terminal

Open your terminal where your Cache binaries are located and follow the below example:

```bash
$ ./cache-wallet
```

That's how simple it really is.
Just loading the program with no added flags is enough for the wallet to connect to your local node.

###### Windows .bat Contents

As stated above, you need to launch the programs via a `.bat` file rather than the standard double-click way that most other programs are launched.
This should be the contents of your `.bat` file:

```bash
cache-wallet.exe
pause
```

That's how simple it really is.
Just loading the program with no added flags is enough for the wallet to connect to your local node.

> [Note] We use a `pause` command within the `.bat` file just in case the cache-wallet fails to load.
> It will pause `cmd` so you're able to clearly see the error.

***

##### Remote Node Conncection

> [Note] When using Windows, you need to launch the client software via a `.bat` file and not by double-clicking or the programs will fail to load.

###### Linux & MacOS Terminal

Open your terminal where your Cache binaries are located and follow the below example:

```bash
$ ./cache-wallet --daemon-address=51.79.100.195:40000
```
By using the flag `--daemon-address` we can connect the wallet to a remote node

###### Windows .bat Contents

As stated above, you need to launch the programs via a `.bat` file rather than the standard double-click way that most other programs are launched.
This should be the contents of your `.bat` file:

```bash
cache-wallet.exe --daemon-address=51.79.100.195:40000
pause
```

By using the flag `--daemon-address` we can connect the wallet to a remote node

> [Note] We use a `pause` command within the `.bat` file just in case the cache-wallet fails to load.
> It will pause `cmd` so you're able to clearly see the error.

***

#### Transfer

Coin's are not meant to be just held.
You can transfer them to other people too for instance if you're paying for goods but don't want to use a public BTC address.

```
[wallet cxcheA]: transfer <privacyLevel> <cxcheAddress> <amount>
```

These are the 3 needed added args to add when you use the `transfer` command.

- <privacyLevel>
  - We use the phrase "Privacy Level" instead of "MixIn" to help normal people understand the option more clearly. Although a user may use **0** for privacy level, the transaction is still private but will be easier to decrypt.
- <cxcheAddress>
  - This is the address you want to send coins to.
- <amount>
  - Amount can be any amount providing you have enough funds to send.

***

#### Backup Wallet

You'll need to write this information down if you want to login to you wallet from a different location or software.

```
[wallet cxcheA]: export_keys
Private spend key: c06b651bafe22a7172410f44615922ee3bee2be9190137340d6f97f63100a309
Private view key: 1a482f111ed040116ed85ef15b9933e776158d8bb15a64486333c4bbe9bddd00
Mnemonic seed: eavesdrop avoid deepest smash uptight guarded assorted wallets duets bifocals eccentric colony talent kiwi hiding puffin agenda dwindling video romance quick nibs riots segments guarded
```

***


