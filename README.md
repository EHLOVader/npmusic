tl;dr: $ npm i npmusic -g && npmusic #hear music, switch any npm with "npmusic" and when it exits, the music stops. Pointless but fun, Mac only for now

I have bad taste in music, happily accepting PRs here: https://github.com/valgaze/npmusic
------------

Just do this:

```sh
npm i -g npmusic && npmusic

```
Note: This will behind the scenes install youtube-dl & mpv if they're not already available

If everything went well (and if it DIDN'T FOR SOME REASON please get in touch) you will hear what tool is all about.


There are few things in life more exhilarating than an npm install. It’s almost like a scene from a movie… which got me thinking and tinkering and $ npmusic was born. 
Once installed, you can run any npm command you want normally but replace “npm” with “npmusic” and music will play in the background while it’s working. You can pick the song if you want or it will pick randomly from a list.
$
$ npm i npmusic -g #install

$ npmusic #play a random song

$ npmusic install #play a random song while running equivalent of $ npm install (music will turn off when done)

$ npmusic -m exciting #play an exciting song

$ npmusic -m budlight install express #play a song by pitbull and install express [alternative --mood moodName]

$ npm music -t #List all moods available

$ npmusic -p  https://www.youtube.com/watch?v=w0N4twV28Mw #Start playing this song in your terminal [alternatively --play url]

$ npmusic -a https://www.youtube.com/watch?v=Ized1XMRp_I #Add this song to the npmusic random rotation [alternatively --add url]


See $ npmusic help for a listing of flags and how to use them


You need node version {{MINIMUM VERSION}} and unfortunately for now, only Mac machines supported

Under the hood uses youtube-dl, mpv for the actual heavy lifting, this is just a thin wrapper

## help
If permissions on your machine are all screwed up (ie you need to run sudo or you have permissions errors), give this a shot: https://docs.npmjs.com/getting-started/fixing-npm-permissions

## Future
1. Add support for Yarn
2. Add support for playlists
3. Update functionality (without requiring users to re-npm install)
4. Rejigger data model
5. set & lock default song
6. More robust (and fun!) logging

## ACTIVELY SOLICITING PULL REQUESTS FOR CONFIG.JSON MOODS. I HAVE TERRIBLE TASTE IN MUSIC
