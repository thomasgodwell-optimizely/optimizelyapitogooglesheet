# optimizelyapitogooglesheet
Guide to setup a poll to the Optimizely API and write the response to Google Sheets

Specifically, these instructions will take the JSON response recieved from the Optimizely REST API and save it to the next blank cell in column A.

1. Open a Google Sheet.
2. Open "Tools" > "Script editor"
3. Paste in the "googlescipt" code
4. Update the url and token variables
5. Press play

To set this script up to run time-based follow these instructions, from the Google Script Editor:

1. Open "Edit" > "Current Project's Triggers"
2. "create a new trigger."
3. Select function "callOpti", select "HEAD", select "Time-driven"
4. Select your type of time based trigger
5. Select your time of day or interval
6. Choose your failure notification settings - this is an e-mail sent to the sheets file owner upon failure

Here is an example of a trigger to run once every minute.
![API Fetch - Project Triggers - Apps Script 2020-04-02 15-47-14](https://user-images.githubusercontent.com/26964971/78257524-3fd82f80-74fa-11ea-8d11-1ebead1719ec.png)
