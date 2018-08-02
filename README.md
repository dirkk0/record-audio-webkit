# record-audio-webkit



I couldn't find a concise example on how to record and playback audio in Safari/Webkit, so I created this git.
It uses a slightly modified version of Daniel Storey's (WebAudioTrack)[https://github.com/danielstorey/WebAudioTrack] library which does all the heavy lifting (thanks, Daniel!).

At the time of this writing, Safari 11 /Mac OSX seems to have a bug leaving about one second of silence at the beginning of the first recording. You can circumvent this bug by making a short recording right at the start.
Surprisingly, this bug doesn't exist on iOS.

- this prevents the 'first time recording silence' issue and challenges the dialog immediately
- uses ```touch-action: manipulation;``` to prevent the zooming effect on iOS