# How To Calculate Game Result

# Download the game's report
- At the "Past Games" section of nika-play.com, enter the desired Game ID in the provided textbox.
- Click the "Download Report" button to download the report.

# Populate CoinID
- At the report, go to the "Ticket" sheet.
- Copy all the coin-ids listed there.
- Append it all to one single string.

# Calculate result
- Hash the coin-ids with SHA-256. We could use some external tool like [this](https://xorbin.com/tools/sha256-hash-calculator).
- Convert the result into decimal representation. [External tool](https://www.rapidtables.com/convert/number/hex-to-decimal.html).
- Take the first to fourth number to form FirstNumber.
- Take the fifth to eighth number to form SecondNumber.
- Take the ninth to twelfth number to form ThirdNumber.
- Take the thirteenth number as JackpotNumber.
- Verify it against the reported result.