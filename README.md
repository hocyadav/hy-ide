# hy-ide
Hariom Yadav IDE
- hocyadav
- hocyadav


    docker run -d \
  --name=chromium \
  --security-opt seccomp=unconfined `#optional` \
  -e PUID=1000 \
  -e PGID=1000 \
  -e TZ=Etc/UTC \
  -e CHROME_CLI=https://www.google.co.in/ `#optional` \
  -p 8080:3000 \
  -p 8081:3001 \
  -v /workspace/linux_google_chrome_login:/config \
  --shm-size="1gb" \
  --restart unless-stopped \
  lscr.io/linuxserver/chromium:latest


