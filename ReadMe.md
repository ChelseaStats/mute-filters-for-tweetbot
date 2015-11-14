#### mute filters for tweetbot

> A bunch of regexes for muting on Tweetbot


###### Follow Friday

+ `(@.*){5}` - mute all tweets containing more than 5 @ mentions.
+ `^((#|@)\S+\s*)+$` - Tweets consisting solely of @usernames and #hashtags, separated by whitespace, with no substantive content
+ `(?i)please.*(\bwatch\b|\bfollow\b)|(\bwatch\b|\bfollow\b).*(me|please|back)` - Follow me, watch me, follow back, watch me please, follow me please etc

###### Check-ins

+ `(?i)checked.*in` - I checked in at...

###### Celebs and crap

+ `\b(?i:B.*ber)\b` — Filter all references to the word Bieber
+ `[D|d]aily [M|m]ail?` - Daily Mail

###### Format

+ `^[A-Z\s\p{P}]*$` - tweets in all caps
+ `\n{6,}` — Posts with 5+ new lines.
+ `(#.*?){6,}` — Posts with 6+ hastags.
+ `#\w{24,}` — Posts that contain long hashtags.
