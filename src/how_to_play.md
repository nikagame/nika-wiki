# How To Play

# Requirement
- [Chia Blockchain wallet](https://github.com/Chia-Network/chia-blockchain)
To play, you don't need Chia Blockchain's full node. Its wallet is sufficient, so make sure to switch to "Wallet Mode" when starting the client. Your wallet address will be used as a Payout Address to receive the prize. If you use an exchange wallet to play, there's no guarantee your prize will land in your account, so DO NOT USE EXCHANGE WALLET.

# Pick the killer number
Choosing the right number is the key point to winning the game. So, use your full mind when picking one. Interpret your dream, look for any hidden sign on your way back from work, calculate your birth constellation or whatever works. The main keyword is never given up trying! Luck will follow you somehow. To get started you could read [this](https://www.eastrohelp.com/blog/lottery-astrology-for-jackpot/) and [that](https://freehoroscopesastrology.weebly.com/blog/astrology-lottery-prediction).

For this guide, let's suppose your name is John Lucky Doe, and your birth date is January 1st, 2001. So, according to [this](https://www.prokerala.com/numerology/lucky-numbers.php):

```
Life Path Number: 5
Destiny Number: 8
Soul Urge Number: 2
Inner Dream Number: 6
Personality Number: 6
```

We could mix and match this number from this information until you get the correct number. If you are the "all or nothing" kind of guy, you could choose all the possible permutations and buy 10 tickets for each number!

Let's say you have this motto in your life:
```
My inner dream would guide my destiny and life path
My soul urge would define my personality
```
You would pick 6852 as a 4-digit number and 6 as a 1-digit jackpot number. Let's proceed with that.

# Check the number availability
Before you buy that killer ticket, it is advised that you check if the number is already reserved or not. So you can manage your expectation and the timing for your luck. To do so, you could go to the "Reserved Ticket" section on nika-play.com.

<!-- <p><img src="images/test_picture.jpg" alt="Reserved Ticket" /></p> -->

Nice! There is no other human being named John Lucky Doe who came to this world at the start of the millennium. Or, he doesn't use the right tool as you do!

Anyway, suppose your other killer number happens to be reserved by another player. In that case, you could still buy the ticket with the same number. You would be joining the waiting list for that number. Your ticket will be purchased immediately when other players' slots run out.

# Buy the ticket

## Get the Chia Address for the number
At the top of nika-play.com, you will see the "BUY YOUR TICKET NOW" box. Input our 4-digit number in the "NUMBER" textbox and our 1-digit number in the "JACKPOT" textbox. And press the "BUY TICKET" button afterward. Copy the resulted address.

<!-- ![](images/testing-test.gif) -->

## Send your XCH with Chia Wallet
- Go to the "SEND" tab in your wallet. 
- Paste the address you get from the previous step in the "Address / Puzzle hash" textbox.
- The price for one ticket is [0.001 XCH](/game_rules.html#2-ticket), so if you want to buy 10 tickets for this number, you will input 0.01 in the "Amount" textbox.
- As for now, there's no definite guide to setting acceptable fees in Chia. According to this [comment](https://github.com/Chia-Network/chia-blockchain/discussions/10379#discussioncomment-2231974), and [comment in the codebase](https://github.com/Chia-Network/chia-blockchain/blob/d87b8ac08766c9cbb4f4577a4819bb592f63123c/chia/full_node/mempool_manager.py#L99), it's safe to input 0.00005 as the fee to make sure our transaction get through.
- Wait for the transaction to become "Confirmed".

# Monitor the transaction
As stated in the [rules](/game_rules.html#9-transaction-confirmations), all transaction need some confirmation before it's get accepted. You could monitor this at "LAST 20 TRANSACTIONS" on the home screen of nika-play.com.

This means our transaction needs 10 confirmations before it gets accepted. If your transaction is already buried by another transaction, you could always search it. The most straightforward term to search is the "To Address" since we know where our fund is sent in advance.

# Verify your ticket
When your transaction has already been accepted, you should see your ticket at "LAST 20 TICKETS" on the home screen of nika-play.com. You could search for it too if you want.

Since current game's [SlotPerNumber](/game_rules.html#7-slotpernumber) is 1, you would only see 1 ticket at this game. You could verify another 9 tickets are reserved for you by going to the "Reserved Ticket" section and searching "6852" in the provided textbox. And then you could come back at the next game to see your ticket automatically purchased for you.

# Wait for the game to end
Besides waiting, you could do what people suggested [here](https://www.quora.com/What-is-the-best-method-of-winning-the-lottery-using-spiritual-methods-Please-read-my-comment-below) (ignore the negative comment!) and then check your Chia Wallet balance afterward. If you did it right and it happened to be one of your many lucky days to win FirstPrize, you would be 3 XCH richer! Now, imagine when the game has 10 [SlotPerNumber](/game_rules.html#7-slotpernumber), you would be 30 XCH richer, just for 0.01 XCH! It means you just double your XCH 3000 times! I love you 3000!

And yes, we haven't talked about [JackpotPrize](/game_rules.html#5-prize) yet, which can be any amount of XCH!

# Keep trying
There's a time when lady luck doesn't come in your favor. Keep that chin of yours up! Like the one American Founding Father, Thomas Jefferson, said:
```
I'm a great believer in luck, 
and I find the harder I work 
the more I have of it.
```