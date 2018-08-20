---
layout: post
title: "How to Make a Simple Twitter Bot"
comments: true
author: "Jason Shu"
tags: [javascript, tutorial]
---

In this tutorial, I'll be walking through how you can build your own Twitter Bot that filters real-time tweets containing a chosen keyword.

If you feel like skipping the tutorial, download the the [source code here](https://github.com/j4sonshu/TwitterBot).
<br><br>

<h3>What You Will Need</h3>
- [Node.js](https://nodejs.org/en/)

- A [Twitter Account](https://twitter.com/i/flow/signup)

- A text editor (I recommend [Sublime Text](https://www.sublimetext.com/))

Before continuing, make sure you have all 3 of these items.
<br><br>

<h3>Create a Twitter App</h3>
1. Apply for a Twitter [developer account](https://apps.twitter.com/). Fill out the application accordingly.

    - **Note:** As of July 2018, you must be approved for a Twitter developer account before you can create apps.

2. Once approved, go back to [Twitter Apps](https://apps.twitter.com/) and click "Create New App".
   <br><br>

<h3>Twitter App Permissions and Keys</h3>
1. s

2. s
   <br><br>

<h3 id="acc">Install Twitter through Node.js </h3>
1. Create a new folder where you want your TwitterBot to go (i.e. Desktop) and give it a name (i.e. TwitterBot).

2. Open up Terminal (macOS) or Command Prompt (Windows).

3. Navigate to your newly created folder using `cd`.

   - For example, if your folder is on the Desktop, type `cd Desktop`, press Enter, type `cd TwitterBot`, and press Enter.

4. Install the `twitter` package by typing `npm install twitter` and pressing Enter.

   - After installation, make sure that `node_modules` is in the folder.

Keep the command line open; we'll need it again later.

Now, let's move onto some code.
<br><br>

<h3>Setting Up the Twitter Object</h3>
1. Open up your favorite text editor.

2. Create a new file and name it `search.js`. Save the file in your TwitterBot folder.

3. Import the `twitter` package we just installed by typing the following code.

   ```javascript
   var TwitterPackage = require("twitter");
   ```

4. Include the keys from before and initialize a new Twitter object.
   ```javascript
   var keys = {
     consumer_key: "", // your keys go in between the quotes
     consumer_secret: "",
     access_token_key: "",
     access_token_secret: ""
   };
   var Twitter = new TwitterPackage(keys);
   ```
5. Set up the stream.

   ```javascript
   Twitter.stream("statuses/filter", { track: "your keyword here" }, function(
     stream
   ) {
     stream.on("data", function(tweet) {
       console.log(tweet && tweet.text);
       console.log("\n");
     });

     stream.on("error", function(error) {
       throw error;
     });
   });
   ```

   Behind the scenes: `'statuses/filter'` tells Twitter we're listening for tweets containing a certain keyword, which is indicated in the second parameter `track:`. Then we output the `tweet` and the tweet's `tweet.text`, to the console. The purpose of `\n` is just to provide a line of space between each tweet for readability.
   <br><br>

<h3>Streaming Real-Time Tweets</h3>
1. Replace `your keyword here` with the word you want to see tweets contain.

    - Make sure it is in between the single quotes.

    - If you want to include multiple keywords, separate words with a comma like so: `keyword1,keyword2`.

2. Go back to command line, which should still be directed at your TwitterBot folder.

   - If you accidentally closed it, go back [here](#acc) follow steps 2-3.

3. Type `node search.js` to run your TwitterBot.
   <br><br>

<h3>Closing Thoughts</h3>
Congrats! You've now created a Twitter Bot using Twitter API.

Again, don't share your Twitter keys to the public!

Read more about the [Twitter Stream API here](https://developer.twitter.com/en/docs/tweets/filter-realtime/guides/basic-stream-parameters.html).