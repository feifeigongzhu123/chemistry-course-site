# 初中 / 高一 / 高二 / 高三化学 · 动画精讲

统一入口：`index.html`（双击打开，本地运行，无需联网）

- 初中化学 33 个知识点 → `junior.html`
- 高一化学 23 个知识点 → `senior.html`
- 高二化学 8 个知识点 → `senior2.html`
- 高三化学 14 个知识点 → `senior3.html`

## 覆盖范围

### 初中 33 点（12 单元）

| 单元 | 知识点 |
|---|---|
| 第一单元 走进化学世界 | 物质的变化和性质、化学实验基本操作 |
| 第二单元 我们周围的空气 | 空气、氧气、制取氧气 |
| 第三单元 物质构成的奥秘 | 分子和原子、原子的结构、元素 |
| 第四单元 自然界的水 | 水的净化、水的组成、化学式与化合价 |
| 第五单元 化学方程式 | 质量守恒定律、如何正确书写化学方程式、利用化学方程式的简单计算 |
| 第六单元 碳和碳的氧化物 | 金刚石、石墨和C60、二氧化碳制取的研究、二氧化碳和一氧化碳 |
| 第七单元 燃料及其利用 | 燃烧和灭火、化学反应中的能量变化、燃料的合理利用与开发 |
| 第八单元 金属和金属材料 | 金属材料、金属的化学性质、金属资源的利用和保护 |
| 第九单元 溶液 | 溶液的形成、溶解度、溶质的质量分数 |
| 第十单元 酸和碱 | 常见的酸和碱、酸碱中和反应 |
| 第十一单元 盐 化肥 | 常见的盐、化学肥料 |
| 第十二单元 化学与生活 | 人类重要的营养物质、化学元素与人体健康、有机合成材料 |

### 高一 23 点（8 章）

| 章 | 知识点 |
|---|---|
| 第一章 物质及其变化 | 物质的分类及转化、离子反应、氧化还原反应 |
| 第二章 海水中的重要元素——钠和氯 | 钠及其化合物、氯及其化合物、物质的量 |
| 第三章 铁 金属材料 | 铁及其化合物、金属材料 |
| 第四章 物质结构 元素周期律 | 原子结构与元素周期表、元素周期律、化学键 |
| 第五章 化工生产中的重要非金属元素 | 硫及其化合物、氮及其化合物、无机非金属材料 |
| 第六章 化学反应与能量 | 化学反应与能量变化（原电池）、化学反应的速率与限度 |
| 第七章 有机化合物 | 认识有机化合物、乙烯与有机高分子材料、乙醇与乙酸、基本营养物质 |
| 第八章 化学与可持续发展 | 自然资源的开发利用、化学品的合理使用、环境保护与绿色化学 |

### 高二 8 点（选择性必修1 / 2）

| 模块 | 知识点 |
|---|---|
| 选择性必修1 化学反应原理 | 化学反应的热效应、化学反应速率、化学平衡、水溶液中的离子平衡、原电池与电解池 |
| 选择性必修2 物质结构与性质 | 原子结构与性质、分子结构与性质、晶体结构与性质 |

### 高三 14 点（选择性必修3 + 专题复习）

| 模块 | 知识点 |
|---|---|
| 选择性必修3 有机化学基础 | 有机化合物的结构与研究方法、烃、烃的衍生物、生物大分子、合成高分子、有机合成与推断、卤代烃与醇酚、醛酮与羧酸酯 |
| 高三专题复习 | 化学实验综合、工业流程与无机综合、化学计算与图像、化学实验基础与安全、化学反应原理综合、物质结构与性质专题 |

每个知识点包含：

- 3 步 2D SVG 动画，器材、现象、粒子、读数均为该点专属；
- 3 段中文语音（Windows Huihui，16 kHz / 16 bit / 单声道），音频结束自动切下一步；
- 进度条由真实播放时间驱动，缓冲/下载时不会先走；切换步骤会先停止上一段音频，不会叠音；
- 播放中可「暂停 / 继续」，暂停后进度条与时间一起冻结；
- 5 道题：初中标「中考真题改编」，高中标「高考真题改编」；4 个选项、逐项解析、可听讲解；
- 每个点 5 题答案覆盖 A/B/C/D，且不会连续两题同答案；
- localStorage 记录已学知识点、答题记录和错题，可重置。

## 语音加载与整学段下载

- 默认按需加载：进入学段不下载音频，播放当前步时才请求该段，并预取下一步。
- 学段首页有「下载本学段语音」按钮：通过浏览器 Cache API 把整个学段的音频缓存到本机，按钮显示进度和已缓存段数；下载完成后再次播放会直接使用缓存，进度条仍与真实播放同步。
- 本地双击 `index.html`（`file://`）时，音频本来就在本机，按钮显示「本地文件 · 无需下载」。
- `localhost` / GitHub Pages 等安全上下文可使用缓存下载；首次进入时不会自动下载整学段，避免手机流量被动消耗。
- 局域网 `http://192.168.x.x` 不是安全上下文，浏览器不允许 Cache API，按钮会提示「需 HTTPS 才能整学段缓存」；此时按需播放、进度同步、暂停仍正常。

## 规模

| | 知识点 | 步数 | 题数 | 语音 | 本地 WAV |
|---|---|---|---|---|---|
| 初中 | 33 | 99 | 165 | 99 段 | 约 86 MB |
| 高一 | 23 | 69 | 115 | 69 段 | 约 61 MB |
| 高二 | 8 | 24 | 40 | 24 段 | 约 21 MB |
| 高三 | 14 | 42 | 70 | 42 段 | 约 36 MB |
| 合计 | 78 | 234 | 390 | 234 段 | 约 204 MB |

## 分享给其他人

音频不是只能在本机播放，它们是普通的静态 WAV 文件，用相对路径 `audio/...` 引用；页面和音频一起分享或部署即可。

1. **离线文件夹（最简单）**：把整个 `chemistry` 文件夹压缩后发给对方，解压后双击 `index.html`。不要单独发 HTML，否则音频缺失。
2. **同一局域网**：在项目目录运行 `python serve.py`，终端会打印本机地址和局域网地址；手机与电脑连同一 Wi-Fi，打开局域网地址即可。
3. **公网静态托管**：把整个文件夹上传到任意静态托管（GitHub Pages、Netlify、内网静态服务器等），入口用 `index.html`。无需后端；音频会按普通静态文件加载。
4. 本地 WAV 合计约 204 MB，上传/分享前如果嫌大，可只发需要的学段或使用 `docs/` 的 MP3 版。

`docs/` 是已经压缩好的发布版：音频转为 16 kHz 单声道 MP3，站点约 40.2 MB，入口仍是 `index.html`；每个学段只在播放时请求当前步的 MP3，不会一次加载全部音频。`chemistry-site.zip` 是同一份站点的压缩包，约 33.2 MB。

## 发布到 GitHub Pages

仓库：`https://github.com/feifeigongzhu123/chemistry-course`
公开站点：`https://feifeigongzhu123.github.io/chemistry-course/`

仓库根目录直接发布 `docs/` 的内容（Pages 源为 `main /`）。更新步骤：

1. 在 GitHub 新建 Token（classic `repo` 或 fine-grained 的 Contents / Pages 写权限）。
2. 把 Token 写入 `D:\AI\ZCode\chemistry\.gh_token`（只放一行）。
3. 运行 `python _build\gh_upload.py`，脚本会建 blob、提交 `main`、等待 Pages 构建并检查首页与 MP3。
4. 成功后删除 `.gh_token`，并到 GitHub 撤销该 Token。

`docs/` 已包含 `.nojekyll`，不需要 Jekyll；音频是静态 MP3，GitHub Pages 直接按普通文件提供。

## 文件

```
index.html             # 统一入口：初中 / 高一 / 高二 / 高三
serve.py               # 局域网静态服务器（python serve.py）
junior.html            # 初中主入口，数据/场景内联
senior.html            # 高一主入口，数据/场景内联
senior2.html           # 高二主入口，数据/场景内联
senior3.html           # 高三主入口，数据/场景内联
data/junior.json       # 初中 33 点课程 + 题库
data/senior.json       # 高一 23 点课程 + 题库
data/senior2.json      # 高二 8 点课程 + 题库
data/senior3.json      # 高三 14 点课程 + 题库
audio/j1-1/step1.wav   # 初中 99 段：j1-*、j2-*、j3-*
audio/s1-1/step1.wav   # 高一 69 段：s1-* ... s8-*
audio/g2-1/step1.wav   # 高二 24 段：g2-1 ... g2-8
audio/g3-1/step1.wav   # 高三 42 段：g3-1 ... g3-14
docs/                  # GitHub Pages 发布版（MP3，约 40.2 MB）
chemistry-site.zip     # docs 的压缩包（约 33.2 MB）
_build/                # 内容、场景 SVG、样式、脚本、TTS、审计
acid-base.html         # 视觉/交互基准
chem-lab.html          # 既有版本，保留
```

## 重新构建

```bat
python _build\build.py          # 初中：data/junior.json + junior.html
python _build\build_senior.py   # 高一：data/senior.json + senior.html
python _build\build_grade.py    # 高二/高三：senior2/senior3 + data
python _build\build_docs.py     # 发布版：docs/（MP3）+ chemistry-site.zip
```

重新生成语音：

```bat
powershell -ExecutionPolicy Bypass -File _build\tts.ps1 -Manifest _build\audio_manifest.json -Root .
powershell -ExecutionPolicy Bypass -File _build\tts.ps1 -Manifest _build\senior_audio_manifest.json -Root .
powershell -ExecutionPolicy Bypass -File _build\tts.ps1 -Manifest _build\g2_audio_manifest.json -Root .
powershell -ExecutionPolicy Bypass -File _build\tts.ps1 -Manifest _build\g3_audio_manifest.json -Root .
```

## 测试

```bat
python _build\audit.py               # 初中数据/页面审计
python _build\audit_grade.py         # 高二/高三数据、音频、页面审计
python _build\audio_check.py         # 初中 99 段音频
python _build\audio_check_senior.py  # 高一 69 段音频
python _build\dom_check.py           # 初中 DOM：JS 错误/点数/场景/题卡/禁用词
python _build\cdp_test.py            # 初中 Edge 无头 + 390px + 答题 + 音频
python _build\cdp_test_senior.py     # 高一 Edge 无头 + 390px + 答题 + 音频
python _build\cdp_test_grade.py      # 高二/高三 390px + 深链 + 答题 + 音频
python _build\cdp_test_docs_grade.py # docs 发布版 MP3 播放检查
python _build\cdp_test_g3b.py       # 高三新增 6 点 390px 验收
python _build\cdp_test_docs_g3b.py  # docs 新增 6 点 MP3/缓存验收
python _build\cdp_audio_test.py     # 进度同步/暂停/切段/整学段缓存
python _build\index_test.py          # 入口页 390px 检查
python _build\serve_test.py          # 静态服务器页面/音频访问检查
python _build\shots_final.py         # 初中验收截图
python _build\shots_senior.py        # 高一验收截图
python _build\shots_g3b.py           # 高三新增 6 点截图
```

题库只做「改编」，不写具体年份或原卷号，避免伪造出处。
