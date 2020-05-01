# Awesome-facebook-LIVE-with-ffmpeg
How To Live Stream Pre Recorded Videos To Facebook Page For Free

How To Stream Live On Facebook Page From ubuntu 18.04 server Using Pre-Recorded Videos

https://www.facebook.com/live/create

ffmpeg -re -y -i output.mp4 -c:a copy -ac 1 -ar 44100 -b:a 96k -vcodec libx264 -pix_fmt yuv420p -vf scale=1080:-1 -r 30 -g 60 -tune zerolatency -f flv -maxrate 2000k -preset veryfast "rtmps://live-api-s.facebook.com:443/rtmp/########################"
