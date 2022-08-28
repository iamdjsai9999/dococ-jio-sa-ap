

### **Installation**:

Clone this repository using
```sh
$ git clone https://github.com/cyberboysumanjay/JioSaavnAPI
```
Enter the directory and install all the requirements using
```sh
$ pip3 install -r requirements.txt
```
Run the app using
```sh
$ python3 app.py
```
Navigate to 127.0.0.1:5000 to see the Homepage

### **Usage**:
Fetching lyrics is optional and is triggered only when it is passed as an argument in the GET Request. (**&lyrics=true**)
**If you enable lyrics search, it will take more time to fetch results**

---
##### **Universal Endpoint**: (Supports Song Name, Song Link, Album Link, Playlist Link)
```sh
http://127.0.0.1:5000/result/?query=<insert-jiosaavn-link-or-query-here>&lyrics=true
```
**Example:** Navigate to http://127.0.0.1:5000/result/?query=alone to get a JSON response of songs data in return.

----


##### **Song URL Endpoint**:
```sh
http://127.0.0.1:5000/song/?query=<insert-jiosaavn-song-link>&lyrics=true
```
**Example:** Navigate to http://127.0.0.1:5000/song/?query=https://www.jiosaavn.com/song/khairiyat/PwAFSRNpAWw to get a JSON response of song data in return.

---

##### **Playlist URL Endpoint**:
```sh
http://127.0.0.1:5000/playlist/?query=<insert-jiosaavn-playlist-link>&lyrics=true
```
**Example:** Navigate to http://127.0.0.1:5000/playlist/?query=https://www.jiosaavn.com/featured/romantic-hits-2020---hindi/ABiMGqjovSFuOxiEGmm6lQ__ to get a JSON response of playlist data in return.

---

##### **Album URL Endpoint**:
```sh
http://127.0.0.1:5000/album/?query=<insert-jiosaavn-album-link>&lyrics=true
```
**Example:** Navigate to http://127.0.0.1:5000/album/?query=https://www.jiosaavn.com/album/chhichhore/V4F3M5,cNb4_ to get a JSON response of album data in return.

---

##### **Lyrics Endpoint**:
```sh
http://127.0.0.1:5000/lyrics/?query=<insert-jiosaavn-song-link-or-song-id>&lyrics=true
```
**Example:** Navigate to http://127.0.0.1:5000/lyrics/?query=https://www.jiosaavn.com/song/khairiyat/PwAFSRNpAWw to get a JSON response of lyrics data in return.

