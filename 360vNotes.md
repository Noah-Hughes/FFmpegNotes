This my notes on using FFmpeg

Upscaling example using lanczos
ffmpeg -i input.mp4 -vf scale=3840x2560:flags=lanczos -c:v libx264 -preset slow -crf 19 output.mp4

https://www.arj.no/2021/12/21/ffmpeg-v360-processing/

Upscaling
https://trac.ffmpeg.org/wiki/Scaling

Hardware acceleration
ffmpeg -y -hwaccel cuda -i input.file output.file

Flaten out video v360
ffmpeg.exe -hwaccel cuda  -i input.mp4 -vf v360=e:flat e-flat.mp4

