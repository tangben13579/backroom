<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>层级列表 - 后室 Wiki</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: "微软雅黑", Arial, sans-serif;
        }
        body {
            background-color: #f0ebe0; /* 仿旧纸张底色 */
            padding: 20px;
        }
        /* 顶部快速跳转栏 */
        .quick-jump {
            background-color: #4a4238;
            color: #fff;
            max-width: 800px;
            margin: 0 auto 20px;
            border: 2px solid #2d2822;
        }
        .quick-jump h3 {
            padding: 8px 12px;
            font-size: 18px;
            border-bottom: 2px solid #2d2822;
        }
        .jump-grid {
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            gap: 2px;
            background-color: #2d2822;
        }
        .jump-grid a {
            display: block;
            background-color: #fff;
            color: #000;
            text-align: center;
            padding: 8px 0;
            text-decoration: none;
            font-size: 14px;
        }
        .jump-grid a:hover {
            background-color: #e0e0e0;
        }
        /* 层级标题栏 */
        .level-header {
            background-color: #4a4238;
            color: #fff;
            max-width: 800px;
            margin: 0 auto;
            padding: 10px 15px;
            border: 2px solid #2d2822;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .level-header h2 {
            font-size: 20px;
        }
        .back-top {
            font-size: 14px;
            color: #fff;
            text-decoration: none;
        }
        /* 层级列表容器 */
        .level-list {
            max-width: 800px;
            margin: 0 auto;
            background-color: #f8f5eb;
            border: 2px solid #4a4238;
            border-top: none;
            padding: 15px;
        }
        .level-item {
            padding: 8px 12px;
            margin: 4px 0;
            background-color: #f0ebe0;
            border-radius: 2px;
        }
        .level-item a {
            color: #b32424; /* 仿红色链接 */
            text-decoration: none;
        }
        .level-item a:hover {
            text-decoration: underline;
        }
        .level-item .sub {
            font-size: 13px;
            color: #666;
            margin-left: 20px;
        }
        .level-item .note {
            font-size: 13px;
            color: #666;
            float: right;
        }
    </style>
</head>
<body>
    <!-- 快速跳转栏 -->
    <div class="quick-jump">
        <h3>快速跳转 📌</h3>
        <div class="jump-grid">
            <a href="#0-99">Level 0-99</a>
            <a href="#100-199">Level 100-199</a>
            <a href="#200-299">Level 200-299</a>
            <a href="#300-399">Level 300-399</a>
            <a href="#400-499">Level 400-499</a>
            <a href="#500-599">Level 500-599</a>
            <a href="#600-699">Level 600-699</a>
            <a href="#700-799">Level 700-799</a>
            <a href="#800-899">Level 800-899</a>
            <a href="#900-999">Level 900-999</a>
        </div>
    </div>

    <!-- Level 0-99 区域 -->
    <div class="level-header" id="0-99">
        <h2>Level 0-99</h2>
        <a href="#" class="back-top">▲ 回到顶部</a>
    </div>
    <div class="level-list">
        <div class="level-item"><a href="#">Level 0 - "教学关卡"</a></div>
        <div class="level-item"><a href="#">Level 1 - "宜居地带"</a></div>
        <div class="level-item"><a href="#">Level 2 - "废弃公共带"</a></div>
        <div class="level-item"><a href="#">Level 3 - "发电站"</a></div>
        <div class="level-item"><a href="#">Level 4 - "废弃办公室"</a></div>
        <div class="level-item"><a href="#">Level 5 - "恐怖旅馆"</a></div>
        <div class="level-item"><a href="#">Level 6 - "熄灯"</a></div>
        <div class="level-item"><a href="#">Level 7 - "深海恐惧症"</a></div>
        <div class="level-item"><a href="#">Level 8 - "岩洞系统"</a></div>
        <div class="level-item"><a href="#">Level 9 - "郊区"</a></div>
        <div class="level-item"><a href="#">Level 10 - "丰裕"</a></div>
        <div class="level-item">
            <a href="#">Level 11 - "无垠城市"</a>
            <div class="sub">↳ 新版: <a href="#">Level 11 - "不夜城"</a></div>
        </div>
        <div class="level-item"><a href="#">Level 12 - "矩阵"</a></div>
        <div class="level-item"><a href="#">Level 13 - "温水煮青蛙"</a></div>
        <div class="level-item"><a href="#">Level 14 - "天堂"</a></div>
        <div class="level-item"><a href="#">Level 15 - "未来走廊"</a></div>
        <div class="level-item"><a href="#">Level 16 - "地形转变"</a></div>
        <div class="level-item"><a href="#">Level 17 - "航空母舰"</a></div>
        <div class="level-item">
            <a href="#">Level 18 - "回忆"</a>
            <span class="note">⚠ 该文章正在重写中</span>
        </div>
        <div class="level-item"><a href="#">Level 19 - "阁楼"</a></div>
        <div class="level-item"><a href="#">Level 20 - "娱乐区 玻瑞阿斯的建筑"</a></div>
        <!-- 可以继续往下添加更多 Level -->
    </div>
</body>
</html>      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
      gap: 18px;
      margin-top: 20px;
    }

    .level-card {
      border: 1px solid #ccc;
      border-radius: 6px;
      overflow: hidden;
      background: #f9f9f9;
      text-decoration: none;
      color: #333;
      transition: 0.2s;
    }

    .level-card:hover {
      transform: translateY(-3px);
      box-shadow: 0 3px 8px rgba(0,0,0,0.1);
      background: #fff;
    }

    .level-card-header {
      background: #0645ad;
      color: white;
      padding: 10px 12px;
      font-weight: bold;
      font-size: 16px;
    }

    .level-card-body {
      padding: 12px;
      font-size: 14px;
    }

    .level-desc {
      margin-bottom: 6px;
    }

    .level-danger {
      color: #d82a2a;
      font-weight: bold;
    }
  </style>
</head>

<body>

<div class="wiki-container">
  <h1 class="page-title">后室 - 层级列表</h1>

  <p>点击任意层级卡片，即可进入该层级的详细介绍。</p>

  <div class="level-grid">

    <!-- Level 0 卡片 -->
    <a href="level-0.html" class="level-card">
      <div class="level-card-header">Level 0 — 入门室</div>
      <div class="level-card-body">
        <div class="level-desc">潮湿的黄色墙纸，无限的空房间</div>
        <div class="level-danger">安全度：较安全</div>
      </div>
    </a>

    <!-- Level 1 卡片 -->
    <a href="level-1.html" class="level-card">
      <div class="level-card-header">Level 1 — 宜居地带</div>
      <div class="level-card-body">
        <div class="level-desc">黑暗仓库，有物资与杏仁水</div>
        <div class="level-danger">安全度：一般</div>
      </div>
    </a>

    <!-- Level 2 卡片 -->
    <a href="level-2.html" class="level-card">
      <div class="level-card-header">Level 2 — 管道噩梦</div>
      <div class="level-card-body">
        <div class="level-desc">狭窄管道，高温与噪音</div>
        <div class="level-danger">安全度：危险</div>
      </div>
    </a>

    <!-- Level 3 卡片 -->
    <a href="level-3.html" class="level-card">
      <div class="level-card-header">Level 3 — 发电站</div>
      <div class="level-card-body">
        <div class="level-desc">巨大机房，物资丰富</div>
        <div class="level-danger">安全度：极危险</div>
      </div>
    </a>

    <!-- Level 4 卡片 -->
    <a href="level-4.html" class="level-card">
      <div class="level-card-header">Level 4 — 废弃办公室</div>
      <div class="level-card-body">
        <div class="level-desc">死寂的空办公室</div>
        <div class="level-danger">安全度：较安全</div>
      </div>
    </a>

  </div>
</div>

</body>
</html>
