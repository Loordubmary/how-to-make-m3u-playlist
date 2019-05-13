# How to make M3U playlist

M3u files to queue files for playback in Multimedia players

# Index

1. About .M3U
2. Uses of .M3U
3. How to make .M3U playlist
4. Sample playlist

# About .M3U

M3U or **M**oving **P**icture Experts Group Audio Layer **3**

M3U is a de facto standard with extension .m3u.

M3U file is a plain text file that specifies the path of one or more media files.

Each entry carries one media path. The media path can be referred by the following ways:

- localpath
	- e.g., C:\My Music\Heavysets.mp3 (External Folder)
	- e.g. Heavysets.mp3 (Internal Folder)
- URL
	- e.g., http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ElephantsDream.mp4


# Uses of .M3U

M3U file format is used to creating a single-entry playlist file pointing to a stream on the Internet or local files.

It is used to make playlist tracks.

It implementation is very easy.

# How to make .M3U playlist

The M3U files is use # character for include extension.

It uses two extension for create playlist. They are listed out in the following,

1. #EXTM3U
2. #EXTINF

# #EXTM3U

It is file header. It is a default one for creating M3U playlist.

The playlist is start from this line. Without this we cannot start playlist.

### Example:

```
#EXTM3U
```

# #EXTINF

This is used to Add file path to the playlist.

This is also used tracking all information about the playlist like filename, duration and title.

### Example:

```
#E#EXTINF:191,Artist Name - Track Title
```

# Sample playlist

### Sample 1

```
#EXTM3U

#EXTINF:123, BigBuckBunny - BigBuckBunny
http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4

#EXTINF:321,ElephantsDream - ElephantsDream
http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ElephantsDream.mp4
```

### Sample 2

```
#EXTM3U

#EXTINF:123, BigBuckBunny - BigBuckBunny
http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/images/BigBuckBunny.jpg

#EXTINF:321,ElephantsDream - ElephantsDream
http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/images/ElephantsDream.jpg
```
