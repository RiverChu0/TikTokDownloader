<div align="center">
<img src="static/images/TikTokDownloader.png" alt="TikTokDownloader" height="256" width="256"><br>
<h1>TikTokDownloader</h1>
<a href="https://github.com/JoeanAmier/TikTokDownloader/blob/master/license">
<img src="https://img.shields.io/github/license/JoeanAmier/TikTokDownloader" alt="GNU General Public License v3.0">
</a>
<a href="https://github.com/JoeanAmier/TikTokDownloader/releases/latest">
<img src="https://img.shields.io/github/v/release/JoeanAmier/TikTokDownloader" alt="TikTokDownloader">
</a>
<a href="https://sourcery.ai">
<img src="https://img.shields.io/badge/Sourcery-enabled-ffd900" alt="Sourcery">
</a>
<img src="https://img.shields.io/github/stars/JoeanAmier/TikTokDownloader?color=green" alt="stars">
<a href="https://github.com/JoeanAmier/TikTokDownloader/blob/master/docs/QQ%E7%BE%A4%E8%81%8A.jpg">
<img src="https://img.shields.io/badge/QQ%E7%BE%A4%E8%81%8A-830227445-ba79b1" alt="群聊">
</a>
</div>
<br>
<p>🔥 <b>TikTok 视频/图集/原声；抖音视频/图集/直播/原声/合集/评论/账号/搜索/热榜数据采集工具：</b>完全开源，基于 Requests 模块实现；批量下载抖音账号发布页或者喜欢页的作品；单独下载抖音链接或 TikTok 链接对应的作品；获取抖音直播推流地址；下载抖音直播视频；采集抖音作品评论数据；批量下载抖音合集作品；采集抖音账号详细数据；采集抖音用户 / 作品搜索结果；采集抖音热榜数据。</p>
<hr>

# 📝 功能清单

* ✅ 下载抖音无水印视频/图集
* ✅ 下载 TikTok 无水印视频/图集
* ✅ 批量下载抖音账号发布页/喜欢页作品
* ✅ 单独下载抖音链接作品
* ✅ 单独下载 TikTok 链接作品
* ✅ 支持单次输入多个链接
* ✅ 多账号批量下载作品
* ✅ 自动跳过已下载的文件
* ✅ 持久化保存采集数据
* ✅ 下载动态/静态封面图
* ✅ 获取抖音直播推流地址
* ✅ 下载抖音直播视频
* ✅ Web UI 交互界面
* ✅ 采集抖音作品评论数据
* ✅ 批量下载抖音合集作品
* ✅ 记录点赞收藏等统计数据
* ✅ 筛选作品发布时间
* ✅ 可实现作品增量更新
* ✅ 支持使用代理采集数据
* ✅ 支持局域网远程访问
* ✅ 采集抖音账号详细数据
* ✅ 作品统计数据更新
* ✅ 自动更新账号昵称
* ✅ 部署至私有服务器
* ✅ 部署至公开服务器
* ✅ 采集抖音搜索结果
* ✅ 采集抖音热榜数据
* ✅ 记录已下载作品 ID
* ☑️ 采集账号关注列表
* ☑️ 批量下载抖音账号收藏作品
* ☑️ 采集抖音账号收藏合集列表

# 💻 程序界面

**终端命令行模式：**
<br><br>
![终端模式截图](docs/终端模式截图1.png)
*****
![终端模式截图](docs/终端模式截图2.png)
<br><br>
**Web UI 交互模式：**
<br><br>
![WebUI模式截图](docs/WebUI模式截图1.png)
*****
![WebUI模式截图](docs/WebUI模式截图2.png)

# 📈 项目状态

* 🟢 [Releases](https://github.com/JoeanAmier/TikTokDownloader/releases/latest) 发布的源码已通过测试，功能均可正常使用
* 🟡 准备开发获取账号关注列表功能
* 🟡 准备开发批量下载账号收藏作品功能
* 🟡 准备开发获取账号收藏合集列表功能
* 🔴 最新版本的源码可能存在不稳定的 Bug
* 🔴 如果在使用过程中发现 Bug，请及时告知作者修复

# 📁 项目结构

```text
TikTokDownloader
├─ main.py                                 // 项目程序启动入口
├─ requirements.txt                        // 程序所需第三方模块信息
├─ settings.json                           // 运行参数配置文件
├─ src                                     // 项目模块源码文件夹
│    ├─ CookieTool.py                      // Cookie 写入模块
│    ├─ Configuration.py                   // 配置文件处理模块
│    ├─ DataAcquirer.py                    // 接口数据获取模块
│    ├─ DataDownloader.py                  // 作品文件下载模块
│    ├─ FileCache.json                     // 文件管理缓存数据
│    ├─ FileManager.py                     // 作品文件管理模块
│    ├─ Parameter.py                       // 加密参数生成模块
│    ├─ Recorder.py                        // 日志及数据记录模块
│    ├─ StringCleaner.py                   // 非法字符处理模块
│    ├─ main_complete.py                   // 终端命令行模式启动入口
│    ├─ main_server.py                     // 服务器部署模式启动入口
│    └─ main_web_UI.py                     // Web UI 交互模式启动入口
├─ cache                                   // 缓存数据文件夹
├─ static                                  // 静态资源文件夹
├─ templates                               // HTML 模板文件夹
└─ docs                                    // 项目文档文件夹
```

# 📋 程序说明

**快速入门：**

<ol>
<li>安装不低于 <code>3.10</code> 版本的 <a href="https://www.python.org/">Python</a> 解释器</li>
<li>下载最新源码或 <a href="https://github.com/JoeanAmier/TikTokDownloader/releases/latest">Releases</a> 发布的源码至本地</li>
<li>安装 requirements.txt 包含的第三方模块</li>
<li>运行 main.py 并选择 <code>终端命令行模式</code>，生成默认配置文件</li>
<li>使用浏览器打开抖音网页版，复制全部 <a href="https://github.com/JoeanAmier/TikTokDownloader/blob/master/docs/Cookie%E6%95%99%E7%A8%8B.md">Cookie</a> 至剪贴板</li>
<li>再次运行 main.py，选择 <code>写入 Cookie 信息</code> 模式，按照提示将 Cookie 写入配置文件</li>
<li>返回程序界面，依次选择 <code>终端命令行模式</code> --> <code>单独下载链接作品</code></li>
<li>输入抖音或 TikTok 作品链接即可下载作品文件</li>
</ol>

<b>
<a href="https://github.com/JoeanAmier/TikTokDownloader/wiki/TikTokDownloader-Documentation">点击查看项目完整文档</a>
</b>

<hr>

**关于 Cookie：**

[点击查看 Cookie 获取教程](https://github.com/JoeanAmier/TikTokDownloader/blob/master/docs/Cookie%E6%95%99%E7%A8%8B.md)

|   程序功能   | 是否需要登录 |
|:--------:|:------:|
| 下载发布页作品  |   ⭕    |
| 下载喜欢页作品  |   ⭕    |
|  下载链接作品  |   ❌    |
| 获取直播推流地址 |   ❌    |
|  下载直播视频  |   ❌    |
| 获取作品评论数据 |   ⭕    |
|  下载合集作品  |   ❌    |
|  获取账号数据  |   ❌    |
|  采集搜索结果  |   ❌    |
|  采集热榜数据  |   ❌    |

**程序获取数据失败时，可以尝试使用已登录的 Cookie 运行！**

<hr>

**其他说明：**

* 程序提示用户输入时，直接回车代表返回上级菜单，输入 `Q` 或 `q` 代表结束运行
* 由于获取账号喜欢页数据仅返回喜欢作品的发布日期，不返回点赞日期，因此程序需要获取全部喜欢作品数据再进行日期筛选，如果账号喜欢页作品较多，可能会花费较长的时间
* 使用 `SQLite` 格式储存数据时，重复获取作品数据将会更新点赞收藏等统计数据
* 获取私密账号的发布页数据需要登录后的 Cookie，且登录的账号需要关注该私密账号
* 批量下载账号作品或合集作品时，如果对应的昵称或标识发生变化，程序会自动更新已下载作品文件名称中的昵称和标识
* 程序下载文件时会先将文件下载至临时文件夹，下载完成后再移动至储存文件夹；程序运行结束时会清空临时文件夹

# ⚠️ 免责声明

<ul>
    <li>
        使用者对本项目的使用由使用者自行决定，并自行承担风险。作者对使用者使用本项目所产生的任何损失、责任、或风险概不负责。
    </li>
    <li>
        本项目的作者提供的代码和功能是基于现有知识和技术的开发成果。作者尽力确保代码的正确性和安全性，但不保证代码完全没有错误或缺陷。
    </li>
    <li>使用者在使用本项目时必须严格遵守 <a href="https://github.com/JoeanAmier/TikTokDownloader/blob/master/license">GNU
        General Public License v3.0</a> 的要求，并在适当的地方注明使用了 <a
            href="https://github.com/JoeanAmier/TikTokDownloader/blob/master/license">GNU General Public License
        v3.0</a> 的代码。
    </li>
    <li>
        使用者在任何情况下均不得将本项目的作者、贡献者或其他相关方与使用者的使用行为联系起来，或要求其对使用者使用本项目所产生的任何损失或损害负责。
    </li>
    <li>
        使用者在使用本项目的代码和功能时，必须自行研究相关法律法规，并确保其使用行为合法合规。任何因违反法律法规而导致的法律责任和风险，均由使用者自行承担。
    </li>
</ul>
<b>在使用本项目的代码和功能之前，请您认真考虑并接受以上免责声明。如果您对上述声明有任何疑问或不同意，请不要使用本项目的代码和功能。如果您使用了本项目的代码和功能，则视为您已完全理解并接受上述免责声明，并自愿承担使用本项目的一切风险和后果。</b>

# 💡 代码参考

* https://github.com/Evil0ctal/Douyin_TikTok_Download_API
* https://github.com/Johnserf-Seed/TikTokDownload
* https://github.com/davidteather/TikTok-Api
* https://requests.readthedocs.io/en/latest/
* https://dormousehole.readthedocs.io/en/latest/
* https://github.com/B1gM8c/X-Bogus
* https://github.com/aithedev/X-Bogus
* https://html5up.net/hyperspace
