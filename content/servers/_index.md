+++
title = "Servers"
chapter = true
weigth = 100
+++

# Servers

| Server | Function |
| ---    | ---      |
| RAW | Primary shell server, mounts fs0, runs main website and space. |
| DPS0 | Digiplay server. Runs digiplay website, stores audio, runs marceline and javo. |
| FS0 | Primary file server. Runs LDAP Samba server, stores user files, webcam images. Runs webcam service. |
| wp-gw | Streaming server. Runs the icecast server which outputs the main audio stream and the sue stream. |
| LOG1/2 | Logs all the audio from the Studio 1 desk. Runs Darkice which gives Icecast on wp-gw the audio to broadcast. |
| VM1 | ??? |