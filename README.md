# subreddit_imgur_picture_downloaderV1.1
Package that takes a subreddit name as an argument and takes all the hot posts, finds imgur links, and downloads them to a specified folder

************IN THE NEW VERSION*************
1. Welcome print out
2. Now supports gfycat gif and webm downloads

## SET UP & INITIAL CONSIDERATIONS BEFORE RUNNING 
1. This is written for Python 2, not 3. I have not checked it in Python 3, but given backwards compatibility issues between 2 and 3, I doubt it will work in 3. I plan to test it and update the code for Python 3 in the near future.
2. you will need to to a `pip install praw` - currently there are some imported packages that are not required. But praw is a must, also urllib2 if you don't already have it. Remember, on OSX and Unix based systems, you may need to `sudo pip install praw`
3. You will need to go to line 49 of the RedditScraper.py file and change the variable `call5` to reflect your desired download location. In the next version this will not be required.
4. You will also need to set up a config file with your Reddit API access credentials. A good tutorial for this is here: https://www.youtube.com/watch?v=krTUf7BpTc0 and I have included an example config where you can fill in the blanks.

That's about it for set up. 

## RUNNING
This script is intended to run off of the bash shell only and will not work in windows command prompt. I have only tested it in OSX so far, but there shoul dbe no issues running it on other unix based systems.
The basic commpand is:

  `python RedditScraper.py <ENTER NAME OF SUBREDDIT>`
  
for example:

  `python RedditScraper.py Art`
  
## ACKNOWLEDGEMENTS

A small part of this was influenced by leonardicus' code for imagur. His command line python code for straight imgur downloads was highly significant to the creation of this code abd influenced the building of my program. I have added additional functionality to it. Now included is support for gifs and webms from Gfycat.


## FUTURE ADDITIONS
1. Test this code in Python 3 and update as necessary to produce a Python 3 version
2. In version 1.2 I will remove unused imports
3. In version 1.2 I will allow users to pass in a specific download location on the command line, for now this must be hard coded into the core package file
4. I will be producing a version compatible for Windows users

## COPYRIGHTS & USE NOTICE
I, the owner of this GitHub account and creater of the subreddit_imgur_picture_downloader, retain all copyrights.
Copyright (C) Simon Augustus - All Rights Reserved.
This program is free to use, but must not be sold. Use of thise code for any commercial purposes is strictly forbidden.
The use of this code in other open source projects must be cleared with the author.
Written by Simon Augustus <augustus.writer@gmail.com>, July 2017
