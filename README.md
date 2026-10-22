# TikTok Mass Downloader

A Node.js script that mass-downloads TikTok videos from a single user profile, without a watermark, together with their descriptions. Give it a profile URL and it saves every video into a folder named after the user; give it a number and it stops after that many videos.

## About

TikTok Mass Downloader (TMD) uses Puppeteer to open a TikTok profile and work through its videos one by one. Each video is downloaded without a watermark (unless the creator re-uploaded it with one burned in), and the video descriptions are collected into a `names.txt` file next to the videos.

## Features

- Downloads all videos from a single TikTok profile in one run
- Optional limit: pass a number to download only that many videos
- Videos saved without a watermark
- Descriptions saved to `names.txt`
- Videos organized in a folder named after the profile (`@username`)

## Requirements

- Node.js

## Installation

```bash
git clone https://github.com/xsrazy/Tiktok-Mass-Downloader
cd Tiktok-Mass-Downloader
npm i
```

## How to Use

Automatic, from the terminal:

```bash
node TMD https://www.tiktok.com/@username
```

Or download only a set number of videos (replace `n` with the count):

```bash
node TMD https://www.tiktok.com/@username n
```

Manual: edit the profile URL inside the `TMD.js` script (or the URL and count in the variant scripts) and run it.

Results are saved with the videos in the `@username` folder and the descriptions in `names.txt`.

## Notes

- Mass downloading can use a lot of data and disk space, depending on how many videos the profile has
- The repository also contains two variant scripts (`Hiu.js` and `Hiu2.js`) alongside the main `TMD.js`
- `package.json` lists the license as ISC while the LICENSE file in this repository is MIT; the LICENSE file is the one that applies

## Credits

Created by [Xsrazy](https://github.com/xsrazy).

## License

MIT License. See [LICENSE](LICENSE) for details.

<a href="https://www.buymeacoffee.com/xsrazy" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
