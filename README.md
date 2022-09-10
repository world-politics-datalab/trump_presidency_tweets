# An Archive of Donald Trump's Tweets Posted During His Presidency
This repository includes the 30,367 tweets posted by President Trump during his presidency. The first tweet was recorded on starting on January 20, 2017 on the morning of the inaguration. The last one was posted on January 8, 2021 shortly before Twitter closed his account for violating its terms of service.

These tweets were extracted from the [Trump Twitter Archive](https://www.thetrumparchive.com/).The CSV file includes 16 variables:

- **source**: This variable informs which platform was used to post the tweet. Possible answers include: "Twitter for iPhone", "Twitter Media Studio" and so forth.

- **text**: The tweet's original text, which in many cases include URLs, emojis and other characters.

- **created_at**: This column includes the date and time the tweet was posted, recorded as POSIXct class.

- **retweet_count**: This variable tell us how many users retweeted the tweet.

- **favorite_count**: This variables informs us how many users favorited the tweet.

- **is_retweet**: This dummy variable captures whether this is an organic tweet (e.g., FALSE) or it is retweet of another user's tweet (e.g., TRUE).

- **id_str**: This is a unique string that Twitter provides to each tweet.

- **date**: Using the =split function Google Sheets, we extracted the date formated as month/day/year from the **created_at** variable.

- **time**: Using the =split function in Google Sheets, we extracted the time the tweet was posted from the **created_at** variable. The time is formatted as hour, minute, second.

- **hour**: Using the =hour function in Googlee Sheets, I extracted from the **time** variable the hour of the day  the tweet was posted.

- **month**: Using the =month function in Google Sheet, I extrated the month number from the **date** varialble.

- **day**: Using the =weekday function in Google Sheet, I extrated the week day number from the **date** varialble.

- **year**: Using the =year function

- **week_number**: Using the =weeknum function in Google Sheet, it informs the reader in what week of the year was the tweet posted.

- **is_rt**: Using a =RegExMatch function in Google Sheets, it specifies if the text starts with "RT" which Twitter uses to inform the user that this is re-tweet. 

- **lower_text**, Using the =lower function in Google Sheets, all words of the text are turned into lower case.
