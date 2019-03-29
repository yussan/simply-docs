## About 
This is api docs to get search video by video id on Youtube Api V3. 
Reference : https://developers.google.com/youtube/v3/docs/search/list


## Request
#### Endpoint : https://www.googleapis.com/youtube/v3/search
#### Method : GET
#### Query parameters :
- key : <string> your_key (required), generate it via Google Console https://console.cloud.google.com/
- order : <string> one of :  date, rating, relevance, title, videocount, viewcount (default is date)
- channelId : <string> id of spesific Youtube channel (optional)
- maxResults : <number> max results per page
- type : <string> one of : video, channel, playlist 
- pageToken : <string> (optional) get next page

### Sample Request
```
https://www.googleapis.com/youtube/v3/search?order=date&part=snippet&channelId=UCc0sgRlqAJCWejiiSIDJjdg&maxResults=5&key=<YOUR_KEY>&type=video
```

## Response
#### Type data : JSON
### Sample Response
```
{
    "kind": "youtube#searchListResponse",
    "etag": "\"XpPGQXPnxQJhLgs6enD_n8JR4Qk/YQXvoGeDKmHBwY1x-pBxL4KjcCw\"",
    "nextPageToken": "CAUQAA",
    "regionCode": "ID",
    "pageInfo": {
        "totalResults": 14,
        "resultsPerPage": 5
    },
    "items": [
        {
            "kind": "youtube#searchResult",
            "etag": "\"XpPGQXPnxQJhLgs6enD_n8JR4Qk/6zxn0AzEdDFwE-3lEFS9xBDoUcI\"",
            "id": {
                "kind": "youtube#video",
                "videoId": "ZF6Su4sl4Lw"
            },
            "snippet": {
                "publishedAt": "2019-03-24T14:49:05.000Z",
                "channelId": "UCc0sgRlqAJCWejiiSIDJjdg",
                "title": "Memilih Mounting Untuk Cyclo Comp",
                "description": "Video ini memberikan review singkat seputar 3 macam mounting untuk cyclo comp yang paling banyak tersedia di pasaran. Nah semoga membantu kamu ...",
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
                    }
                },
                "channelTitle": "Mau Gowes",
                "liveBroadcastContent": "none"
            }
        },
        {
            "kind": "youtube#searchResult",
            "etag": "\"XpPGQXPnxQJhLgs6enD_n8JR4Qk/BwQ0nGAdiRlIFNuS85PuwlvauCE\"",
            "id": {
                "kind": "youtube#video",
                "videoId": "dfYSxqijDFc"
            },
            "snippet": {
                "publishedAt": "2019-03-21T14:57:13.000Z",
                "channelId": "UCc0sgRlqAJCWejiiSIDJjdg",
                "title": "Review Topeak Race Rocket HP - Pompa Kecil Bertekanan Tinggi",
                "description": "Jadi cerita minggu kemarin saya mengalami ban bocor di daerah Batul, DIY. Perjalanan kira - kira sudah sekitar 30Km dari rumah, nah waktu itu saya tak bawa ...",
                "thumbnails": {
                    "default": {
                        "url": "https://i.ytimg.com/vi/dfYSxqijDFc/default.jpg",
                        "width": 120,
                        "height": 90
                    },
                    "medium": {
                        "url": "https://i.ytimg.com/vi/dfYSxqijDFc/mqdefault.jpg",
                        "width": 320,
                        "height": 180
                    },
                    "high": {
                        "url": "https://i.ytimg.com/vi/dfYSxqijDFc/hqdefault.jpg",
                        "width": 480,
                        "height": 360
                    }
                },
                "channelTitle": "Mau Gowes",
                "liveBroadcastContent": "none"
            }
        },
        {
            "kind": "youtube#searchResult",
            "etag": "\"XpPGQXPnxQJhLgs6enD_n8JR4Qk/SX8ZF-WA972QhNak6BY_HOrtIhk\"",
            "id": {
                "kind": "youtube#video",
                "videoId": "fQcq0MTkrGY"
            },
            "snippet": {
                "publishedAt": "2019-03-19T04:46:16.000Z",
                "channelId": "UCc0sgRlqAJCWejiiSIDJjdg",
                "title": "Panduan Mengganti Ban Dalam Road BIke",
                "description": "Ban bocor adalah hal yang paling dihindari oleh semua pesepeda, namun meskipun belum pernah mengalaminya, bisa jadi dimasa depan baik itu kamu atau ...",
                "thumbnails": {
                    "default": {
                        "url": "https://i.ytimg.com/vi/fQcq0MTkrGY/default.jpg",
                        "width": 120,
                        "height": 90
                    },
                    "medium": {
                        "url": "https://i.ytimg.com/vi/fQcq0MTkrGY/mqdefault.jpg",
                        "width": 320,
                        "height": 180
                    },
                    "high": {
                        "url": "https://i.ytimg.com/vi/fQcq0MTkrGY/hqdefault.jpg",
                        "width": 480,
                        "height": 360
                    }
                },
                "channelTitle": "Mau Gowes",
                "liveBroadcastContent": "none"
            }
        },
        {
            "kind": "youtube#searchResult",
            "etag": "\"XpPGQXPnxQJhLgs6enD_n8JR4Qk/lCLOEHdNMDzo4rvyvxbN4kBhhDo\"",
            "id": {
                "kind": "youtube#video",
                "videoId": "mMvIh562H2Q"
            },
            "snippet": {
                "publishedAt": "2019-03-04T03:10:31.000Z",
                "channelId": "UCc0sgRlqAJCWejiiSIDJjdg",
                "title": "Tips Membuat Jalur Bersepeda Menggunakan Google Maps",
                "description": "Kamu biasanya kalo membuat jalur bersepeda dan share teman-teman menggunakan metode apasih. Ada banyak sih opsinya, bisa mulut ke mulut, gambaran, ...",
                "thumbnails": {
                    "default": {
                        "url": "https://i.ytimg.com/vi/mMvIh562H2Q/default.jpg",
                        "width": 120,
                        "height": 90
                    },
                    "medium": {
                        "url": "https://i.ytimg.com/vi/mMvIh562H2Q/mqdefault.jpg",
                        "width": 320,
                        "height": 180
                    },
                    "high": {
                        "url": "https://i.ytimg.com/vi/mMvIh562H2Q/hqdefault.jpg",
                        "width": 480,
                        "height": 360
                    }
                },
                "channelTitle": "Mau Gowes",
                "liveBroadcastContent": "none"
            }
        },
        {
            "kind": "youtube#searchResult",
            "etag": "\"XpPGQXPnxQJhLgs6enD_n8JR4Qk/PEAZupcG8YwuqZU2WHcNJHi6r-E\"",
            "id": {
                "kind": "youtube#video",
                "videoId": "vpAByeNe-3A"
            },
            "snippet": {
                "publishedAt": "2019-02-26T02:33:30.000Z",
                "channelId": "UCc0sgRlqAJCWejiiSIDJjdg",
                "title": "Cara Menggabung Aktivitas Strava Yang Terpotong",
                "description": "Apa kadang kamu merasa jengkel jika tiba-tiba aktifitas Strava terpotong dan harus buat baru. Nah dengan cara ini kamu bisa menggabungkan semua aktifitas ...",
                "thumbnails": {
                    "default": {
                        "url": "https://i.ytimg.com/vi/vpAByeNe-3A/default.jpg",
                        "width": 120,
                        "height": 90
                    },
                    "medium": {
                        "url": "https://i.ytimg.com/vi/vpAByeNe-3A/mqdefault.jpg",
                        "width": 320,
                        "height": 180
                    },
                    "high": {
                        "url": "https://i.ytimg.com/vi/vpAByeNe-3A/hqdefault.jpg",
                        "width": 480,
                        "height": 360
                    }
                },
                "channelTitle": "Mau Gowes",
                "liveBroadcastContent": "none"
            }
        }
    ]
}
```
