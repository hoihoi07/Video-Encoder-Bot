# Video-Encoder-Bot
 a telegram bot for compressing/encoding videos in h264 format.

### Configuration
Add values in environment variables or add them in [config.env.example](/VideoEncoder/config.env.example) and rename file to `config.env`.

**Basics**
- `API_ID` - Get it by creating an app on [https://my.telegram.org](https://my.telegram.org)
- `API_HASH` - Get it by creating an app on [https://my.telegram.org](https://my.telegram.org)
- `BOT_TOKEN` - Get it by creating a bot on [https://t.me/BotFather](https://t.me/BotFather)

**Authorization**
- `SUDO_USERS` - Chat identifier of the sudo user. For multiple users use space as seperator.

**Encode Settings**
- `PRESET` - [https://telegra.ph/Encode-Settings-Guide-11-22](https://telegra.ph/Encode-Settings-Guide-11-22)
- `TUNE` - [https://telegra.ph/Encode-Settings-Guide-11-22](https://telegra.ph/Encode-Settings-Guide-11-22)
- `AUDIO` - [https://telegra.ph/Encode-Settings-Guide-11-22](https://telegra.ph/Encode-Settings-Guide-11-22)

**Optional**
- `UPLOAD_AS_DOC` - (Optional) Uploads Video as doc if `True` else `False`.
- `DOWNLOAD_DIR` - (Optional) Temporary download directory to keep downloaded files.
- `ENCODE_DIR` -(Optional) Temporary encode directory to keep encoded files.

### Configuring Encoding Format
To change the ffmpeg profile edit them in [ffmpeg.py](/VideoEncoder/utils/ffmpeg.py)

### Deployment
With python3.7 or later.
```
pip3 install --no-cache-dir -r requirements.txt
python3 -m VideoEncoder
```
### Deploy To Heroku
- [https://heroku.com/deploy?template=https://github.com/hoihoi07/Video-Encoder-Bot](https://heroku.com/deploy?template=https://github.com/hoihoi07/Video-Encoder-Bot)
### Credits
- [ShannonScott](https://gist.github.com/ShannonScott) for [transcode_h265.py](https://gist.github.com/ShannonScott/6d807fc59bfa0356eee64fad66f9d9a8)
- [viperadnan-git](https://github.com/viperadnan-git/video-encoder-bot) for queue etc.

### Copyright & License
- Copyright &copy; 2021 &mdash; [WeebTime](https://github.com/WeebTime)
- Licensed under the terms of the [GNU AFFERO GENERAL PUBLIC LICENSE](./LICENSE)
