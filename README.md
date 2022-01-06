This is a fork of janus-gateway by meetecho.

Currently I added a feature to the plugins.streaming module.
The feature is called 'RTSP-on-demand'. The goal is not to waste a traffic
between the RTSP server and Janus gateway when there are no clients viewing the stream. 
There is a new configuration parameter 'rtsp_on_demand = true|false (default false)'.
If you set rtsp_on_demand to true, rtsp stream will be disconnected
when there are no more webrtc clients left.
