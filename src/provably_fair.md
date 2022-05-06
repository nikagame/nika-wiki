# Provably Fair

Anyone can repeatedly calculate every result in Nika games, but the result is always consistent. There's no way to know the outcome of future games, hence Provably Fair.

As stated in the [rules](/game_rules.html#2-ticket), a player must buy a ticket to participate in Nika games. Ticket purchasing happens in the Chia blockchain, which produces a unique Coin ID. So each game will have its own set of Coin IDs. To calculate the game result, one has to append all the Coin IDs for the said game (in hex format, with 0x prefix), then hash it with SHA-256. Take the hash result in decimal representation, and then:

- FirstNumber = First to the fourth character of the result.
- SecondNumber = Fifth to the eighth character of the result.
- ThirdNumber = Ninth to the twelfth character of the result.
- JackpotNumber = Thirteenth character of the result.

Learn how to prove it [here](/how_to_calculate_game_result.html).