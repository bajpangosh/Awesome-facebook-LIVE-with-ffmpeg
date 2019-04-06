# Awesome-facebook-LIVE-with-ffmpeg
How To Live Stream Pre Recorded Videos To Facebook Page For Free

How To Stream Live On Facebook Page From ubuntu 18.04 server Using Pre-Recorded Videos

https://www.facebook.com/live/create

ffmpeg -re -y -i 1.mp4 -c:a copy -ac 1 -ar 44100 -b:a 128k -vcodec libx264 -pix_fmt yuv420p -vf scale=720:-1 -r 30 -g 60 -f flv "rtmp://rtmp-api.facebook.com:80/rtmp/xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
