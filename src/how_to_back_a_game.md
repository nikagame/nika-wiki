# How To Back A Game

# Requirement
- [Chia Blockchain wallet](https://github.com/Chia-Network/chia-blockchain)
To back the game, you don't need Chia Blockchain's full node, and its wallet is sufficient, so make sure to switch to "Wallet Mode" when starting the client. Your wallet address will be used as a Payout Address to receive the profit reward. If you use an exchange wallet to back the game, there's no guarantee your profit share will land in your account, so DO NOT USE EXCHANGE WALLET.
- Chia balance > 6 XCH
Please read this to figure out why we choose six.
- [Discord](https://discord.com/) account
We value privacy and anonymity, so we use Discord as the mean of communication between the backer and our server. We only collect user IDs and usernames from your account and will not share them with any party. 

# Join our server
Please make sure you have already joined our server. There is where your adventure for profit begins.

# Summon the bot
In the "general" channel, summon the bot by sending:
```
!bot
```
The bot will approach you by a direct message to start interacting with you. Or, if you want to avoid any suspicion of your account, you could DM-ing the bot directly. They (yes, this bot declaring their pronouns as they/them) would respond appropriately.

# Ask for a top up address
Now you have slid in the bot's DM, send:
```
backer start
```
to get started. This friendly bot would respond to ask you to wait while they notice our server to get a unique Chia address just for you.

# Choosing your backing amount
While you are waiting for that excellent bot, here is some consideration to choose how much you would commit to back the game. As you may already know, when you dedicate 6 XCH, you create 1 SlotPerNumber in the game, but it doesn't mean the amount must be a multiplier of six. You could choose any amount above 6 to increase your share of the game's profit.

# Send the XCH
After you decide how many XCH you will send, hopefully, the bot has already come back with your address. Now it's time to send it to start back the game.
- Go to the "SEND" tab in your wallet. 
- Paste the address you get from the bot in the "Address / Puzzle hash" textbox.
- Input your chosen amount in the "Amount" textbox.
- As for now, there's no definite guide to setting acceptable fees in Chia. According to this [comment](https://github.com/Chia-Network/chia-blockchain/discussions/10379#discussioncomment-2231974), and [comment in the codebase](https://github.com/Chia-Network/chia-blockchain/blob/d87b8ac08766c9cbb4f4577a4819bb592f63123c/chia/full_node/mempool_manager.py#L99), it's safe to input 0.00005 as the fee to make sure our transaction get through.
- Wait for the transaction to become "Confirmed".

# Monitor the transaction
As stated in the [rules](/nika-wiki/game_rules.html#9-transaction-confirmations), all transaction need some confirmation before it's get accepted. You could monitor this at "LAST 20 TRANSACTIONS" on the home screen of nika-play.com.

This means our transaction needs ten confirmations before it gets accepted. If another transaction already buries your transaction, you could always search it. The most straightforward term to search is the "To Address" since we know where we sent our fund in advance.

But, if you don't have time for this, worry none. That excellent bot will inform you when your fund is accepted.

# Enjoy the profit
We can't guide you on how to do this tough. You can add another yacht to your collection, claim 70% of Google's ownership, or create a full-blown casino. But you could always buy a Nika's game ticket to make a game more exciting and potentially double your "already colossal" profit. 

# Monitor your backing activity
While you are busy spending that never-ending profit, you could get a recap of your backing activity by contacting the bot again. Just type:
```
backer info
```
They will calculate all the information regarding your contribution to the games. 

# Increase your backing amount
We understand your insatiable ambition. Please don't feel bad about it. You could always send more XCH to your given address to make your profit even more prominent!

# Withdraw your backed fund
When time is hard, you can always withdraw your backed fund. In the next game, you would lose some reward (or all your reward if you release all your funds). Please type:
```
backer withdraw <your_amount_in_mojo>
```
Replace `<your_amount_in_mojo>` with the amount you want to withdraw. Your fund will be sent to your wallet when the current game ends.

And then, when life gets easier again, you could always send the Chia address to be a great backer once again. A backer account is never expired.