# TikTokDownloader

批量下载账号发布页或者喜欢页的视频和图集，或者单独下载分享链接的视频和图集。

# Settings.json

|   参数   |  类型  |                                          说明                                          |
|:------:|:----:|:------------------------------------------------------------------------------------:|
|  url   | str  |                                   账号主页分享链接，批量下载时使用                                   |
|  mode  | str  |                    批量下载类型，post 代表发布页，like 代表喜欢页<br>（需要账号喜欢页公开可见）                     |
|  root  | str  |                                   文件保存路径，默认值：当前路径                                    |
| folder | str  |                单独下载分享链接的资源时，保存的文件夹名称<br>（如果文件夹不存在会自动创建，默认值：Download）                 |
|  name  | str  | 文件保存时的命名规则，值之间使用空格分隔，默认值：发布时间-作者-描述<br>id: 唯一值；desc: 描述；create_time: 发布时间；author: 作者 |
|  time  | str  |                       发布时间的格式，默认值：年-月-日（注意：Windows下文件名不能包含“:”）                       |
| split  | str  |                                   文件命名的分隔符，默认值：“-”                                   |
| music  | bool |                                是否下载视频和图集的音乐，默认值：False                                |

# 参考

* https://github.com/Johnserf-Seed/TikTokDownload
* https://requests.readthedocs.io/en/latest/
