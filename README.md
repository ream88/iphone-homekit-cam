- Request the NDI SDK from https://www.ndi.tv/sdk/. An email will be sent to you.
- Download the linked file.
- Extract the SDK:

  ```
  docker run -it --rm -v $(pwd):/home -w /home debian:stretch-slim /home/InstallNDISDK_v4_Linux.sh
  ```

- Move the extracted SDK into `docker-ffmpeg-ndi`:

  ```
  mv "NDI SDK for Linux" docker-ffmpeg-ndi
  ```

- Build the Docker image:

  ```
  docker build -t ffmpeg-ndi docker-ffmpeg-ndi
  ```
