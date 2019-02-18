# Streaming

### Does LiveSYNC support live streaming?

At the moment all videos and contents must be copied to the director and all audience devices before you start presenting contents. In LiveSYNC it is possible to stream contents if you provide URLs in JSON format. 

The JSON includes only three fields: **name**, video **url** and an optional field **layout** which tells video projection. The layout can be any of the following types: "2D" , "360" , 360TB" , "360SBS" .

    {
        "name":"Yle",
        "url":"http://yletv-lh.akamaihd.net/i/yletv1hls_1@103188/master.m3u8",
        "layout":"2D"
    }

Save the JSON file with the .videostream extension, for example, myvideo.videostream.  This works the way that LiveSYNC doesn't download the file to the memory, instead it plays it live from the Internet. 

LiveSYNC works for live broadcasts, if you just copy a Vimeo or YouTube stream link to the .videostream file, then it might only work for a short period of time until the service generates new links. If so, make sure you update the link to the .videostream file with newly generated link/s. With Vimeo Pro, this is not a problem, because links are made to stay as they are just for cases like this.