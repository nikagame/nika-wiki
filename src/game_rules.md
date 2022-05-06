# Game Rules

Game in Nika is a form of play in predefined set of time which player try to guess some number which will appear at the end of the game, and will get the reward if their guess is correct.

# 1. Duration
1. Each game in Nika lasted 120 minutes.
2. Timezone used is UTC.
2. There can't be two or more games running simultaneously. It's always one game at a given time.
# 2. Ticket
1. One ticket is worth 1000000000 Mojo (0.001 XCH). 
2. One ticket contains one 4-digit number and a 1-digit jackpot number.
3. To play in Nika, one has to buy the ticket(s).
4. Each player can buy the ticket(s) as many as they like, but it will be limited by the game's [SlotPerNumber](#7-slotpernumber).
5. The Chia blockchain address used to buy a ticket would be used as the player's payout address to receive any prize.
# 3. Result
1. Each game would output three pairs of a 4-digit number and one 1-digit number. We call the resulted pair as FirstNumber, SecondNumber, and ThirdNumber. And one 1-digit number is called JackpotNumber.
2. Each result pair could have duplicated a 4-digit number.
3. Result is calculated using [provably fair](/provably_fair.html) algorithm based on Chia blockchain's Coin ID.
# 4. Win Condition
1. Player is declared the winner if their ticket's number matches the game result.
2. There is four types of a winner, FirstWinner, SecondWinner, ThirdWinner, and JackpotWinner.
3. FirstWinner is whose ticket's 4-digit number matches FirstNumber.
4. SecondWinner is whose ticket's 4-digit number matches SecondNumber.
5. ThirdWinner is whose ticket's 4-digit number matches ThirdNumber.
6. JackpotWinner is the FirstWinner whose ticket's 1-digit matches JackpotNumber.
7. If the game's SlotPerNumber is more than one, it's possible to have multiple winners in each type.
8. Since a player could buy more than one ticket, then it's possible for one player to declare as every winner type.
# 5. Prize
1. FirstWinner would be rewarded 3000000000000 Mojo (3 XCH).
2. SecondWinner would be rewarded 2000000000000 Mojo (2 XCH).
3. ThirdWinner would be rewarded 1000000000000 Mojo (1 XCH).
4. JackpotWinner would be rewarded by any XCH available in Jackpot Pool Prize.
5. When there are multiple FirstWinner, SecondWinner, and ThirdWinner in one game, each of them would be rewarded the full amount according to their winning type.
6. When there are multiple JackpotWinner in one game, the reward from Jackpot Pool Prize would be distributed equally among JackpotWinners.
7. Every prize is immediately sent to the winner's payout address after the game end.
8. At the end of each game, the jackpot pool prize is calculated first according to [Ticket Sales Allocation](/ticket_sales_allocation.html), then distributed to the JackpotWinners for that game, if there are any.
# 6. Backer
1. Each game needs at least one eligible backer to be started. When there is none, then the game will not start.
2. Backer is declared eligible when they commit 6000000000000 Mojo (6 XCH) or more.
3. Any profit or loss that happens in one game would be distributed according to their backing amount.
4. Profit sharing reward immediately sent to backer's payout address after the game end.
5. Backer would take loss sharing from their committed XCH after the game end.
6. Withdrawal of committed XCH would be processed and sent to the backer's payout address after the game end.
7. Backer's committed amount would be recalculated at the end of the game, so their eligibility may be changed in the next game.
# 7. SlotPerNumber
1. SlotPerNumber is calculated before the game starts and will not change until the game is finished.
2. SlotPerNumber is calculated by dividing the game's backed amount by the total prize amount, which is 6000000000000 Mojo (6 XCH).
3. If the divide operation has a remainder, it will be floored.
# 8. Reserved Ticket
1. Reserved ticket is automatically created when a player purchases a ticket for the 4-digit number already bought up to the current game's SlotPerNumber.
2. Reserved tickets would be used to purchase a ticket with the same number in the next games.
3. Ticket purchasing from reserved tickets would be executed before the game.
4. Coin ID used to calculate a game result for the ticket purchased by the reserved ticket is the Coin ID for the original transaction.
5. Reserved ticket is sorted by the transaction height in the Chia blockchain. The smaller the height, the sooner it will be executed.
# 9. Transaction Confirmations
1. Confirmation means the Chia's block where the transaction happened is buried with another block.
2. The more considerable the amount, the more confirmation is needed for transactions confirmed by the game.
3. For any transaction below 1 XCH, ten confirmation is needed.
4. For any transaction above or equal to 1 XCH, the following rules apply:
```
minConfirmation = ((amountInMojo / 10000000000000) + 2) * 10
Divide operation executed as integer division, which means the result is floored.
```

