These are two files written in Intersystems Cache. They haven't been touched for several years so 
this is mainly to show an example of what Cache can look like.

They are three programs I wrote a while ago when first checking out Cache.

ZDANZAT is the main program for creating a message. It is basically a chat application that runs on a cache instance.
  It takes the entire terminal window, and other people in the same cache instance (or environment,
  its been a while) can see messages that others send. It works by checking for updates to one of 
  those global hashes (I don't recall the exact term for them) that may have been posted by another
  user. There are a few special commands, one of which deletes the shared variable and the files related to the
  app itself.

ZHELLOWC is the viewing window. This is where all the messages written by users are posted (so to use the app fully
  you need to have two terminals open in the same environment). 

XRACECAR2 is a simple race car game that runs in the terminal. One of the options in the chat app is
  to jump into the game and play. Once the user hits a wall, they end up back in the chat app and a notice
  gets echoed to the other users regarding the score.


There may or may not be dependencies that your environment may or may not have, and I don't intend on fixing any of that.
This is here more of as a "here is what Cache looks like" than as a fully working thing (however feel free to try and use it
at your own risk in a dev environment, but you should probably not use this in prod.)
