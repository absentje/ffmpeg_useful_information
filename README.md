# ffmpeg_useful_information

## Check available devices: (for example: ip cameras, ip microphones):
ffmpeg -list_devices true -f dshow -i dummy

example output:

[dshow @ 0000021dd0f2d440] DirectShow video devices (some may be both video and audio devices)

[dshow @ 0000021dd0f2d440]  "A4tech HD 720P PC Camera"

[dshow @ 0000021dd0f2d440]     Alternative name "@device_pnp_\\?\usb#vid_09da&pid_2697&mi_00#7&56ddd4&0&0000#{65e8773d-8f56-11d0-a3b9-00a0c9223196}\global"

## Show camera stream from ffplay:
ffplay -f dshow -i video="A4tech HD 720P PC Camera"
