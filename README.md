Audio Player app for the Nokia 81104G - [Gerda](https://gerda.tech/) 

### Features
audio player and podcast downloader


### Manual
+ **Cursor up/down** file navigation 
+ **Enter** play selected file
+ **Enter long press** delete selected file
+ **Soft-key-left** pause
+ **Soft-key-right** volume
+ **key 1** add selected file to playlist
+ **key 4** play playlist
+ **key 5** jump to next folder
+ **key 2** jump to previous folder
+ **key 7** download podcasts

### Podcast downloader
Put on your sd card a file with the name audio.json with the following structure:


```
[
	
		{
			"url":"http://www.ndr.de/podcast/podcast3008.xml",
			"episods":"2",
			"dir":"ndr"
		},

		{
			"url":"http://podcast.wdr.de/radio/leonardo.xml",
			"episods":"2"
			"dir":"wdr"
		},

	

		{
			"download_path":"/storage/sdcard/podcast/"

		}
	
]

```

Create the root podcast dir manually for example /storage/sdcard/**podcast**/

be very careful when specifying the download path: "download_path": "/storage/sdcard/podcast/"
because it can happen that if you set the wrong download path overrides your system
do a test before with adb shell!!

### to do

- add id3 tag-reader to create more readable file names
- delete old podcast episods
- loop
⁻ when playing big files >100mb crash the app 

### Thank you
https://tutorials.de and https://groups.google.com/forum/#!forum/bananahackers
