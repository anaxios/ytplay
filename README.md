# ytplay

```
Usage: ytplay [-s QUERY] [-c CHANNEL_NAME] [-p VIDEO_ID] [-n NUMBER] [-r RATE] [-b BROWSER] [-f] [-h]

A thin yt-dlp/vlc wrapper for searching and playing YouTube videos,
with optional local caching.

Options:
  -s QUERY         Search YouTube for QUERY and prompt for a video to play.
  -c CHANNEL_NAME  Search a specific channel.
  -p VIDEO_ID      Play a specific YouTube video by its ID.
  -n NUMBER        Number of search results to fetch with -s (default: ${NUMBER}).
  -r RATE          Playback rate passed to vlc's --rate option.
  -b BROWSER       Read cookies from BROWSER via yt-dlp's
                   --cookies-from-browser (e.g. chrome, firefox, safari).
  -f               Play in fullscreen (vlc --fullscreen).
  -h               Show this help message and exit.

Environment:
  YTPLAY_CACHE       Directory used to cache downloaded videos.
                     If unset, videos are streamed and not cached.

Examples:
  ytplay -n 10 -s "lofi hip hop"
  ytplay -f -r 1.5 -p dQw4w9WgXcQ
  ytplay -b firefox -s "talk"
  ytplay -b firefox -c "theesotericachannel" -s "platonism"

```
