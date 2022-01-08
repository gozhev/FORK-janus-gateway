This is a fork of janus-gateway by meetecho.

I added a feature called 'RTSP-on-demand' to the plugins.streaming module.
The goal is not to waste a traffic between the RTSP server and Janus gateway
when there are no clients viewing the stream. 

There is a new configuration parameter 'rtsp_on_demand = true|false (default false)'.
If you set rtsp_on_demand to true, the RTSP stream will be disconnected
each time there are no more webrtc clients left.
