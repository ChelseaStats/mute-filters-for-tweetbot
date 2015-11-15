#### Mute Filters for Tweetbot

> A bunch of regexes for muting on Tweetbot, the popular iOS/Mac twitter app.
> It is recommended you test regexes with some tweet text (tweetbot lets you copy a tweet's text, paste it here) on regexr.com

##### Check-ins, social sites user requests etc

+ `(?i)checked.*in` - I checked in at...
+ `LinkedIn` - Linked In
+ `(?i)please.*(\bwatch\b|\bfollow\b)|(\bwatch\b|\bfollow\b).*(me|please|back)` - Follow me, watch me, follow back, watch me please, follow me please etc

##### Celebs 

+ `([B|b]ieber)|([B|b]ieb)` — Filter all references to the word Bieber
+ `\b([B|b]eckham)\b` — Filter all references to the word Beckham

##### Media
+ `[D|d]aily [M|m|F|f]ail?|Mail Online|dailym.ai` - Daily Mail/Fail
+ `#[A|a]sk\w*` - Any Ask [celeb] 
+ `([X|x] [F|f]actor|[X|x][F|f]actor|#x[F|f]actor)` - x factor
+ `#[E|e]urovision\w*` - Eurovision
+ `#FIFA\w*` - Fifa (including the game)
+ `#GBBO\w*` - Great British Bake Off
+ `#BakeOff\w*` - Great British Bake Off
+ `#BAFTA\w*` - Bafta
+ `#BGT\w*` - Britains Got Talent
+ `#BBC\w*` - BBC hashtag
+ `#[B|b]allon\w*` - Ballon d'or
+ `#(Glasto|GLASTO|glasto)\w*` - Glastonbury
+ `#ssnhq\w*` - Sky Sports News Hashtags
+ `#[V|v]ote\w*` - Vote hashtags

##### Format

+ `^[A-Z\s\p{P}]*$` - tweets in all caps
+ `\n{6,}` — Posts with 6+ new lines.
+ `(#.*?){6,}` — Posts with 6+ hastags.
+ `#\w{24,}` — Posts that contain long hashtags.
+ + `(@.*){5}` - mute all tweets containing more than 5 @ mentions.
+ `^((#|@)\S+\s*)+$` - Tweets consisting solely of @usernames and #hashtags, separated by whitespace


##### Apps (mute clients)

+ SumAll
+ SumAll Authentication
+ Twitter Ads
+ Unfollowers
+ Unfollowers.me
+ Untappd
+ LinkedIn
+ JustUnfollow
+ Foursquare
+ fllwrs
+ Deezer
+ BreatheSport
+ Bloglovin
