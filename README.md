Flexcoin
========

Source code for Flexcoin digital currency.  First to have easy to use digital Vault to secure coins
https://bitcointalk.org/index.php?topic=260234.msg2776110#msg2776110

Crypto currency is the coolest innovation ever.  But why aren't crypto currencies being adopted by everyone?  The reason is that security is really difficult for the users.  The best security we have right now are paper wallets, and they are really clunky to use.   We need to make the process of securing coins completely painless for the end user.  To do that we need to introduce a few new concepts.  

Vaults:  The first new concept is a vault.   All this is is a device that is always disconnected from the internet so that it can't be hacked.   This is where the private keys and all the coins are stored.   This device can either be a Raspberry Pi, or a computer.   The Vault device needs to be NFC (near field communications) enabled.   This allows the user to take thier cell phone, and touch it to the Vault to top off thier Wallet.  This is called doing a Sync.

But what is to prevent the Wallet from getting hacked so that it tricks the Vault into releasing all of it's coins to the Wallet?  We need another new concept to handle this.

Denominated Addresses: These are addresses which are capable of only holding a fixed amount of Flexcoins.  For example, a 100 Flexcoin address can only hold 100 Flexcoins, or 0 Flexcoins once they have been spent.  There are still regular addresses that can hold any amount of coins but those are for Wallets, not Vaults.

The user logs on to the Vault to set the maximum number of coins that can be releasd in a single Sync.  

Sync:  There are a number of things that need to happen during a Sync. The first thing is to top off a wallet that has a low balance.  The user tells the wallet what balance it should maintain.    Say 200 Flexcoins.  Suppose the wallet is empty.  When the user touches their cell phone to the Vault, the Wallet asks for two 100 coin private keys.  Since this is under the maximim, the Vault sends two 100 FlexCoin private keys.  But we also need the ability to fill the Vault up with coins.   To do this, the Vault has to be capable of generating Public Address/private key pairs.  And it will send out Public Addresses to the Wallet as needed.   

Easy Backups:  The other thing we do is make Vault backups super easy.   Just plug one or a few thumb drives into your Raspberry Pi or Vault computer.  The Vault app will do backups on a regular basis.  The app will be smart enough to automatically keep enough backups over time to ensure full coverage.  Deleting redundant backups. 

So that's pretty much it.  A very simple design that is super easy for the end users.  Just touch your cell phone to the Vault device to top off your wallet while the rest of your coins remain completely safe.  Sure you could lose your cellphone or it's coins could be stolen, but someone could steal your non digital wallet too.   The point is that the amount they can steal is small.

We are looking for developers and other contributors to get in on the ground floor and help make FlexCoin a resounding success.  Reply to this thread if you are interested in joining the team.  There is only one requirement to joining the team, that you treat everyone involved with the FlexCoin team and the broader FlexCoin community with civility and respect, whether they deserve it or not.  The team will decide things like if there should be a premine or not, and how any rewards should be divvied up.
