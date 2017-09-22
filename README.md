# Bloc Jams

Bloc Jams is a static streaming music website that puts all of your favorite tunes in an easy-to-use library. This project was made for [Bloc's Web Development Program](https://www.bloc.io/).

### Music library
All items in the music library are organized through the `scripts/fixtures.js` file. Each album is its own object, with the album cover and songs saved in `assets/images/album_covers` and `assets/music` respectively.
```javascript
var albumNewAlbumNameHere = {
    title: 'Album Title Here',
    artist: 'Album Artist Here',
    label: 'Album Label Here',
    year: 'Album Year Here',
    albumArtUrl: 'assets/images/album_covers/album-artwork-here.png',
    songs: [
        { title: 'First Album Song', duration: 161.71, audioUrl: 'assets/music/first-song-here' },
        { title: 'Second Album Song', duration: 103.96, audioUrl: 'assets/music/second-song-here' },
        { title: 'Third Album Song', duration: 268.45, audioUrl: 'assets/music/third-song-here' },
        { title: 'Fourth Album Song', duration: 153.14, audioUrl: 'assets/music/fourth-song-here' },
        { title: 'Fifth Album Song', duration: 374.22, audioUrl: 'assets/music/fifth-song-here' }
    ]
};
```
_Please note: Song duration is written in seconds. This is required for proper formatting of time played/time remaining in the player bar._

### Buzz! library
Bloc Jams relies on the [Buzz! library](https://buzz.jaysalvat.com/) to play and pause music. A number of Buzz methods manage audio file playback, inlcuding `.play()`, `.pause()`, `.stop()`, `isPaused()`, etc.

### Bloc Jams Angular
To see this project reworked with the Angular framework, check out my [Bloc Jams Angular](https://github.com/karakarakaraff/bloc-jams-angular) repository.
