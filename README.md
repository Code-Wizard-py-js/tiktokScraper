# The Unofficial GUI for the Unofficial TikTokApi

Provides a user friendly interface for the [Unofficial TikTok Api](https://github.com/davidteather/TikTok-Api). Allows you to download your liked videos, videos from the trending page, user uploads, and more.



<sup>Also, I haven't cleaned up the code yet so don't judge me okay.. </sup>

![demo](https://github.com/DeeFrancois/tiktok-scraper-gui/blob/main/DocumentationImages/demo.gif)

## Motivation
I use TikTok for language learning and stumbled upon the very useful [Unofficial TikTok Api](https://github.com/davidteather/TikTok-Api) while looking for a way to download the videos. Figured it would be more efficient to use if it had an interface. Initially, I was just focused on downloading TikTok likes, but then I kept wanting to add more and more features to create a more complete and intuitive experience. I was also interested in getting experience with collaberating on a Github project, although I don't feel this is polished enough to share yet.

## External dependencies
- ffmpeg - https://www.ffmpeg.org/download.html
- mpv - https://github.com/jaseg/python-mpv
- youtube-dl - https://github.com/ytdl-org/youtube-dl

## Python dependencies
- opencv
- Pillow
- python-mpv
- TikTokApi
- youtube_dl

You can just use pip to install them with the requirements.txt file provided



Your JSON file should consist of a list of cookies formatted like so:
```
    {
    "domain": ".tiktok.com",
    "expirationDate": XXXXXXXXXXXXXXXX,
    "hostOnly": false,
    "httpOnly": false,
    "name": "passport_csrf_token",
    "path": "/",
    "sameSite": "no_restriction",
    "secure": true,
    "session": false,
    "storeId": "0",
    "value": "XXXXXXXXXXXXXXXXXXXXXXXXXX",
    "origin": "https://www.tiktok.com"
    },
```
Importing your cookies
The API currently has a couple of bugs when it comes to the verification process during data fetching. However, they can be circumvented by providing your own cookies. To do this you will have to log in to the TikTok website, use a browser extension to export your cookies into a JSON file, and place that file in the same folder as the program. Doing this will also allow you to fetch your likes without having to make them public.
## Usage

**Make sure your likes are public, enter your username in the top bar, click Retrieve TikToks**




Licensed under the [MIT License](LICENSE).
