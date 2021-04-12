# github-cheat-sheet
Lage en readme file
```sh
echo "# github-cheat-sheet" >> README.md
```

Lage local repo
```sh
git init
```
ffmpeg -i adobe.mkv -c:a mp3 -q:a 1 adobe.mp3
#-q:a -> variable bit rate

Keep different audio tracks
```
ffmpeg -i adobe.mkv -map 0:1 adobe.mp3 # keep first audio track
ffmpeg -i adobe.mkv -map 0:2 adobe.mp3 # keep second audio track
ffmpeg -i adobe.mkv -c copy -map 0 adobe.mp4 # keep all audio tracks

```

convert to mp4, keep all audio tracks
```sh
ffmpeg -i adobe.mkv -c copy -map 0 adobe.mp4
