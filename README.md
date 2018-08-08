# plugdj-discord
Bot to play music from a plug.dj room to discord 

## How to install

* Clone this repository : `git clone https://github.com/Dazzuh/plugdj-discord ` 
* Open the repository folder : `cd plugdj-discord`
* Install the depencies : `npm install`
* Install [ffmpeg/avconv](https://www.ffmpeg.org/download.html)
* The command ffmpeg/avconv has to be accessible from the command prompt, with libopus enabled in compilation.
* Use `ffmpeg -formats` and check if `opus` appears, build for windows from https://ffmpeg.zeranoe.com/builds/ contains libopus 
* Rename the file `config.json.example` to `config.json`
* Edit the configuration with the required informations, like the discord bot token, the ffmpeg command path (`ffmpeg`), with forceLibOpus enabled
* Start the bot: `npm start`
* Join a voice channel and write the command `<prefix>!plug <roomname>`, ex: `pl!plug nightblue`

### Depencies installation known issues

* Node-opus installation : node-gyp is required to install
* youtube-dl installation: Spawn error exception: It seems that youtube-dl download a wrong version of the binary youtube-dl.exe on windows. Download a good version of the binary [here](https://rg3.github.io/youtube-dl/download.html) and put it in `node_modules/youtube-dl/bin`
