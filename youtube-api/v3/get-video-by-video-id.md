## About 
This is api docs to get data video by video id on Youtube Api V3. 
Reference : https://developers.google.com/youtube/v3/docs/videos/list


## Request
#### Host : https://www.googleapis.com/youtube/v3/videos
#### Method : GET
#### Query parameters :
- key : <string> your_key (required), generate it via Google Console https://console.cloud.google.com/
- id : <string> youtube_video_id
- part : <string> combination / one of : "snippet,statistics"    

### Sample Request
```
https://www.googleapis.com/youtube/v3/videos?id=ZF6Su4sl4Lw&key=<YOUR_KEY>&part=snippet,statistics
```

## Response
#### Type data : JSON
### Sample Response
```
{
    "kind": "youtube#videoListResponse",
    "etag": "\"XpPGQXPnxQJhLgs6enD_n8JR4Qk/YTn2yv00j9kALchnA4adhO-QB_0\"",
    "pageInfo": {
        "totalResults": 1,
        "resultsPerPage": 1
    },
    "items": [
        {
            "kind": "youtube#video",
            "etag": "\"XpPGQXPnxQJhLgs6enD_n8JR4Qk/ICqGT5U4eOpSVrk5fntGbIHNo8g\"",
            "id": "ZF6Su4sl4Lw",
            "snippet": {
                "publishedAt": "2019-03-24T14:49:05.000Z",
                "channelId": "UCc0sgRlqAJCWejiiSIDJjdg",
                "title": "Memilih Mounting Untuk Cyclo Comp",
                "description": "Video ini memberikan review singkat seputar 3 macam mounting untuk cyclo comp yang paling banyak tersedia di pasaran. Nah semoga membantu kamu untuk memutuskan akan menggunakan mounting jenis yang mana ya.",
                "thumbnails": {
                    "default": {
                        "url": "https://i.ytimg.com/vi/ZF6Su4sl4Lw/default.jpg",
                        "width": 120,
                        "height": 90
                    },
                    "medium": {
                        "url": "https://i.ytimg.com/vi/ZF6Su4sl4Lw/mqdefault.jpg",
                        "width": 320,
                        "height": 180
                    },
                    "high": {
                        "url": "https://i.ytimg.com/vi/ZF6Su4sl4Lw/hqdefault.jpg",
                        "width": 480,
                        "height": 360
                    },
                    "standard": {
                        "url": "https://i.ytimg.com/vi/ZF6Su4sl4Lw/sddefault.jpg",
                        "width": 640,
                        "height": 480
                    },
                    "maxres": {
                        "url": "https://i.ytimg.com/vi/ZF6Su4sl4Lw/maxresdefault.jpg",
                        "width": 1280,
                        "height": 720
                    }
                },
                "channelTitle": "Mau Gowes",
                "tags": [
                    "roadbike",
                    "cycling",
                    "sepeda",
                    "bicycle",
                    "maugowes",
                    "cyclo comp",
                    "mounting"
                ],
                "categoryId": "17",
                "liveBroadcastContent": "none",
                "defaultLanguage": "id",
                "localized": {
                    "title": "Memilih Mounting Untuk Cyclo Comp",
                    "description": "Video ini memberikan review singkat seputar 3 macam mounting untuk cyclo comp yang paling banyak tersedia di pasaran. Nah semoga membantu kamu untuk memutuskan akan menggunakan mounting jenis yang mana ya."
                },
                "defaultAudioLanguage": "id"
            },
            "statistics": {
                "viewCount": "46",
                "likeCount": "5",
                "dislikeCount": "0",
                "favoriteCount": "0",
                "commentCount": "2"
            }
        }
    ]
}
```
