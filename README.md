# USE AT YOUR OWN RISK. NOT RESPONSIBLE FOR ANYTHING THAT THIS PROGRAM DOES. PERSONAL USE ONLY. NO COMMERCIAL USE. 

This is a fork of @Kito0615's NetEaseMusicDownloader with some fixes and mods.

### Q&A

Q: What is this?

A: A working downloader to get stuff from NetEase (music.163.com). Edited from https://github.com/Kito0615/NetEaseMusicDownloader. THIS IS A SELF STUDY PROJECT, NO WARRANTY OR ANY SUPPORT WILL BE GIVEN.

Q: How do I use it?

A: 
1. Clone (download) this repo and extract to somewhere.
2. Make sure you have Python 3+ with requests + pycryptodome installed (run "pip3 install requests" and "pip3 install pycryptodome" AFTER you install Python 3) NOTE: If you run into "ModuleNotFoundError: No module named 'Crypto'", follow the instructions here: https://stackoverflow.com/a/58613670
3. Install Lame (from the exe provided), make sure you install it in C:\Windows\System32 (WARNING: MUST HAVE ADMIN ACCESS). 
4. Follow the original usage instructions below, but basically run: "python3.8.exe ./NetEaseMusic.py URL_TO_SONG" (example setup: Windows 10, Python 3.8 installed from Windows Store, cd to .\Downloads\NetEaseMusicDownloader-master\) 
         

Q: I got a problem!

A: Sorry, I'm not the developer of this downloader, ask @Kito0615


All credits to the original devs, I only fixed some errors and stabilized some stuff.


# // ORGINAL README STARTS HERE //

# NetEaseMusicDownloader

[中文说明](https://github.com/Kito0615/NetEaseMusicDownloader/blob/master/README_CN.md) 

> **NOTE:** In this script, I used some api via [AD's API](https://api.imjad.cn/). Thanks. This 
> script is for personal use only. It cannot be used for any commercial 
> activities. All legal issues are not related to the author.
>
> **NOTE**: With new source from [QQMusic](http://y.qq.com) added, the source API is get from ite [webpage](http://y.qq.com), **all right revserved by [QQMusic](http://y.qq.com)**. This was **only for study**.

#### Update: 2019-06-6

1. Fix code.
2. Localization

#### Update:2018-09-06

1. **New version of Downloader.**Add some options for the script.

2. Usage : `python3 NetEaseMusic.py ` `[OPTIONS]` `URL` or `NetEaseMusic`  `[OPTIONS]` `URL`

3. Option List:

   | Option            | Instruction                              |
   | ----------------- | ---------------------------------------- |
   | -h, --help        | Show help message.                       |
   | -s, --single      | Specific the URL is a single music.      |
   | -l, --list        | Specific the URL is a list.              |
   | -v, --video       | Specific the URL is a music video.       |
   | -r, --range RANGE | Specific to download the music in RANGE. |
   |                   | RANGE format like '1, 2, 5-7, 18'        |
   | -a, --auto        | Add to iTunes Library automatically.     |
   | -f, --folder      | Specific the destination folder.         |

#### Update:2018-08-09

1. Add Lame Tag for iTunes.
2. Now offcial web api failed, still using thrid-part API from AD. I will fix this ASAP.

#### Update: 2018-07-17

1. Add API from official website crack.
2. Add song best bit rate detect.

#### Update: 2018-06-14

1. Add ask for "Add to iTunes automatically".
2. Fixed break down when file exists or search in QQMusic failed.

#### Update:2018-05-28

1. Use new non-offcial api which get from the web replaced the old api.

#### Update:2018-05-22:

1. Now you can use this tool to download songs/playlists/albums. Use *AD's API*.
2. Support windows now. 
3. Support NetEaseMusic MV download now.

#### Update:2018-05-17
1. Add new source from [QQMusic](http://y.qq.com) when the song not available with [NetEaseMusic](http://music.163.com).
2. Add new dependencies [FFMPEG](http://ffmpeg.org) for convert source from QQMusic with *.m4a* extension to *.mp3*.

#### Download:

1. **Clone project**

   ```shell
   git clone https://github.com/Kito0615/NetEaseMusic.git	
   ```

   Then you can run script(NetEaseMusic.py) in terminal with python3. Like:

   ```shell
   python3 NetEaseMusic.py
   ```

   or:

   ```shell
   chmod +x NetEaseMusic.py
   ./NetEaseMusic.py
   ```

2. **Download release**

   Click [here](https://github.com/Kito0615/NetEaseMusicDownloader/releases), download the version you need. Then you can run the binary file in terminal like:

   ```shell
   ./NetEaseMusic
   ```

   or copy the binary to `/usr/local/bin`, then you can execute the binary anywhere you want.

   ```shell
   copy NetEaseMusic /usr/local/bin
   NetEaseMusic
   ```


#### Usage:

​	Check [Update:2018-09-06](#update2018-09-06)

#### Envrionment:

[Python3.0+](https://www.python.org/downloads/mac-osx/) (with [*requests*](https://github.com/requests/requests) installed.)

[lame](http://lame.sourceforge.net) (use this lib to add Cover for audio.) [Here](https://github.com/Kito0615/NetEaseMusicDownloader/blob/master/Install_lame.md) is some instructions.

[Homebrew](https://brew.sh/) 

[License](https://github.com/Kito0615/NetEaseMusicDownloader/blob/master/LICENSE)

[FFMPEG](http://ffmpeg.org)
