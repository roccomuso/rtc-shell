# rtc-shell
WebRTC-based Shell.

## Usage

```
rtc-shell -l -x /bin/sh

  Initiate a webrtc connection, printing the base64 introducer blob to stdout.
  Paste the introducer from the other node as the first line on stdin.
  The -x /bin/sh param will execute a shell script and pipe incoming on stdin and output on stdout.

rt-shell

  Connect to an initiated webrtc connection.
  Paste the introducer from the other node as the first line on stdin.
  After pasting the introducer, another introducer will be printed to stdout for
  the remote node to use.

After the introductions, stdin is forwarded to the remote connection and data
from the remote connection goes to stdout.
```

# Author

Rocco Musolino, inspired by substack/rtcat.
