FROM ubuntu

RUN apt update && apt install wget python3 ffmpeg -y
RUN wget https://github.com/yt-dlp/yt-dlp/releases/latest/download/yt-dlp -O /usr/bin/yt-dlp && \
  chmod +x /usr/bin/yt-dlp

CMD /usr/bin/yt-dlp --config-location /config/yt-dlp.conf
