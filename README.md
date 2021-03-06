# Presentation Remote JS
A simple network-based remote control with NodeJS (and [node-key-sender module](https://github.com/garimpeiro-it/node-key-sender), that used in project, uses Java).
Currently, these can be controlled:
+ System volume. (increase, decrease, mute and unmute)
+ Up, Down, Left and Right buttons.
+ PageUp and PageDown buttons.
+ Home and End buttons.

## Usage
If we assume that the program is in the /Path/To/PresentationRemoteJS folder, you must use the following command to run server on `<PORT>` and streaming screen on `<SCREEN-PORT>` port number:
```
node /Path/To/PresentationRemoteJS [-p <PORT>] [-s <SCREEN-PORT>]
```
Then you should see the output that says:
```
Open below address(es) in browser:
http://<IP-ADDRESS>:<PORT>
```
And now you have access to your system from `http://<IP-ADDRESS>:<PORT>` .
Also note that the default server port is `8888` and default screen streaming port is `8787`.

## Note:
Currently, volume controls (increase, decrease, mute and unmute) are only active for Gnu/Linux, MacOS and MS-Windows.
## Note:
I'm not a NodeJS programmer and this is my first project in NodeJS; So this project is not clean and pretty code! I will try to clean it and make it more professional at my leisure time.

## Changes (V. 0.2.0)
+ Screen presenting protocol changed from HTTP to WebSocket.
