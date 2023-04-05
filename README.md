# mediaplayer
* This is a video file player, mainly used in exhibition displays or museums, can be controlled by external sensors (serial port), or network signals, with default list, list switching, custom hover titles and other functions

# of decoders relied on
* Windows version, which relies on the decoding capabilities of WMF.
    * Install additional codecs to support more encoding formats, `LAVFilters` is recommended
* Linux version, which relies on GStreamer's decoding capabilities.
    * Install additional codecs to support more encoding formats, `GStreamer Multimedia Codecs` is recommended
		* Take Debian as an example
		```
		sudo apt-get install gstreamer1.0-pulseaudio
		apt-get install libgstreamer1.0-0 gstreamer1.0-plugins-base gstreamer1.0-plugins-good gstreamer1.0-plugins-bad gstreamer1.0-plugins-ugly gstreamer1.0-libav
		sudo apt-get install libqt5multimedia5-plugins
		```
* Android version, which relies on the decoding power of MediaPlayer.

# Important documents and directories
* The `/video` directory in the path where the program is running
	* If you place a video file in this directory, it will be automatically scanned
		* Need to set `No_list=true`
* The `/video1`~`/video4` directory under the path where the program is running
	* Video directory for additional players
* `config.ini` file under the program run path
	* The program configuration parameters setting file
* The `/list` directory under the program run path
	* Playlist file storage path, playlist name: 0.m3u~9.m3u
		* where `0.m3u` is the default playlist	
# Remote \ local control function
1. Play, pause, stop, replay, previous song, next song, fast forward, fast rewind, volume up, volume down, mute, unmute, show subtitles, hide subtitles
2. Full screen, return to window
3. Toggle playlist 0~9
4. Heartbeat Pack Monitoring
