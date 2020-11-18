# peerflix

Streaming torrent client for Node.js

```
npm install -g peerflix
```

[![build status](http://img.shields.io/travis/mafintosh/peerflix.svg?style=flat)](http://travis-ci.org/mafintosh/peerflix)

## Usage

Peerflix can be used with a magnet link or a torrent file.
To stream a video with its magnet link use the following command.

```
peerflix "magnet:?xt=urn:btih:ef330b39f4801d25b4245212e75a38634bfc856e"
```

Remember to put `"` around your magnet link since they usually contain `&`.
`peerflix` will print a terminal interface. The first line contains an address to a http server. The `--vlc` flag ensures vlc is opened when the torrent is ready to stream.

![peerflix](https://raw.github.com/mafintosh/peerflix/master/screenshot.png)



[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

```
peerflix --help
```

Examples of usage of could be

```
peerflix magnet-link --list # Select from a list of files to download
peerflix magnet-link --vlc -- --fullscreen # will pass --fullscreen to vlc
peerflix magnet-link --mplayer --subtitles subtitle-file.srt # play in mplayer with subtitles
peerflix magnet-link --connection 200 # set max connection to 200
```


## License

MIT
