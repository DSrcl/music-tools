A collection of terminal tools to download music from youtube.
To setup just do `./setup.sh` (might need some priviledge).
### What do they do
* `batch-dl` takes a list of song names and downloads them using youtube-dl.
* `list-spotify` takes a url from Spotify's web UI and lists all all the songtracks in it.
Piping these two programs together allows you to "download" songs from spotify. This is exactly what `spotify-dl` does.
* `set-album` set album allows you to set album name of a mp3 file.

### How to use them
* The usage of `batch-dl` is pretty straight forward. See `batch-dl -h` for help. Same for `set-album`.
* `list-spotify` and `spotify-dl` rely on Spotify's API, so you would need to get an access token to use them. If everything is in place, juse `list-spotify -u [url of album or playlist] will list all the sound tracks in standard output.

### How to get access token from Spotify
1. `list-spotify -r` redirects you to the url to register an app. After registering the app, copy your `client id`, which you would need for next step.
2. `list-spotify -g` redirects you to the url to manually request an `access token`. 
3. `list-spotify -a [access token]` allows you to store `access token` you obtained from last step.
