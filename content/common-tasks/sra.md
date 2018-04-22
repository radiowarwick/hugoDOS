+++
title = "SRA Chart Show"
chapter = true
weight = 101
+++

# Running the SRA Chart Show

To start/end the SRA chart show you need to SSH into the `dps0` server and be using root.

## Starting the stream

1. Kill the liquidsoap program. `pkill liquid soap`
2. Start a new screen session. `screen`
3. Start the host station's stream. `mplayer <url>`
4. Detatch from the screen. Press `CTRL-A` followed by `D`
5. Go away for 2 hours. You can exit your ssh session without worry.

## Ending the stream

1. SSH back into `dps0`
2. Reattatch to the screen session. `screen -r`
3. End mplayer. Press `CTRL-C`
4. Terminate the screen. `exit`
5. Restart the Marceline service. `service marceline restart`