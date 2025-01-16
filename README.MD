# ksh.sysyzx
一个基于手写HTML的纯文本信息发布平台，拥有首页跳转和基于StatiCrypt的访问限制。这是它的Git存储库。
## 项目结构
```
ksh.sysyzx
│  404.html	第一级自定义404页面
│  index.html	首页
│  ksh.sysyzx.txt.json	公告栏（/lp）
│  LICENSE	许可证
│  README	这个文件
│  plana.txt.json	公告栏（/lp/ee）
│
└─lp	着陆页
    │  404.html	第二级自定义404页面
    │  index.html	实际最终页面
    │
    └─ee	远程收信页（仅限科技社社内成员）
            404.html	带有StatiCrypt提示的自定义404页面
            index.html	远程收信页（上传前经过StatiCrypt处理）
```
**为什么使用`.txt.json`而不是`.txt`：**因为这个项目运行在Cloudflare Pages上，它会在浏览器请求TXT文件时将其作为二进制流下载（而不显示）。
## 许可
Copyright (C) 2025 Lark Sinensis; HKEMS-STMO.

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program.  If not, see <https://www.gnu.org/licenses/>.