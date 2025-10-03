<!--
 * @Author       : BNDou
 * @Date         : 2022-10-30 19:12:57
 * @LastEditTime: 2025-08-27 19:45:06
 * @FilePath: \Auto_Check_In\README.md
 * @Description  :
-->
# Add workflows
> 利用Github的Actions替代青龙定时执行任务
- 添加run.yaml文件，执行夸克签到
- 设置参数：COOKIE_QUARK，QYWX_AM
  > COOKIE_QUARK 多账户用 回车 或 && 分开
    user字段是用户名 (可是随意填写，多账户方便区分)
    例如: user=张三; url=https://drive-m.quark.cn/1/clouddrive/act/growth/reward?xxxxxx=xxxxxx&kps=abcdefg&sign=hijklmn&vcode=111111111;

  > QYWX_AM 企业微信应用 可以根据自己的需求设置
- 运行测试
- 成功截图

  ![image](https://im.litscorpi.top/1758827098023.png)

- 青龙通知有字数限制，多账号显示不完全。对msg进行了处理，分段输出。
  
# Auto_Check_In

> 每日自动签到集合

~~小米社区~~ | 掌飞签到 | 掌飞购物 | 掌飞寻宝 | speed大乐透 | 夸克网盘 | 人人视频 | 小米运动 | 恩山论坛 | ~~必应搜索~~

## 更新日志
- 2025-08-27 因 **掌飞寻宝** 活动更新，原脚本不适配，该功能暂时移除，修复时间暂无法确定，请耐心等待
- 2025-01-09 合并 **签到**、**购物**、**寻宝** 功能到 **掌上飞车全能版（多线程）**
    1. 添加多线程支持，实现多账号并行执行
    2. 添加实时进度条显示
    3. 优化消息推送格式
    4. 添加功能控制参数（具体参数请查看脚本注释）
    5. 完善错误处理和提示
- 2024-08-05 新增 speed端游-周末大乐透 系列工具
- 2024-07-15 修复 夸克网盘自动签到
- ~~2024-07-14 修复 【测试版】夸克网盘自动签到~~
- 2024-06-12 新增 掌飞扫码登录 获取cookie关键属性(参数只适用于签到脚本)
- 2024-05-10 新版掌飞V4 签到已更新
- 新版掌飞V3 签到、掌飞购物、掌飞寻宝、掌飞开金丝篓已修复

## 青龙部署

1. 拉库指令（拉库失败请自行添加代理）

```
ql repo "https://github.com/BNDou/Auto_Check_In.git" "checkIn_" "backUp" "utils" "main" "py"
```

2. 根据"**_代码文件头部注释_**"或者"**_运行提示_**"添加对应的"**_环境变量_**"

## 捐赠支持，用爱发电

<a href="https://github.com/BNDou/"><img height="200px" src="https://cdn.bndou.eu.org/gh/BNDou/Auto_Check_In/readme/donate.jpg" /></a>

您的赞赏，激励我更好的创作！谢谢~

个人维护开源不易，本项目的开发与维护全都是利用业余时间。

如果觉得我写的程序对你小有帮助，或者

想投喂 `雪王牌柠檬水 * 1`

那么上面的微信赞赏码可以扫一扫呢

赞赏时记得留下【`GitHub昵称`】和【`留言`】

### 捐赠榜

| 用户 | 平台 |
|:---:|:---:|
| Citizen Z | WeChat |
| 钟情于 | WeChat |
| M | WeChat |
| [Struggle-best](https://github.com/Struggle-best) | WeChat |
| [Machae1](https://github.com/Machae1) | WeChat |
| [AfanChang](https://github.com/AfanChang) | WeChat |
| [1983shake](https://github.com/1983shake) | WeChat |
| [mmmmm1mm](https://github.com/mmmmm1mm) | WeChat |
| [qqsmms](https://github.com/qqsmms) | WeChat |

## 技术鸣谢
- [Chiupam](https://github.com/chiupam)
- [Cp0204](https://github.com/Cp0204)

## 免责声明
- 这里的脚本只是自己学习 python 的一个实践。
- 仅用于测试和学习研究，禁止用于商业用途，不能保证其合法性，准确性，完整性和有效性，请根据情况自行判断。
- 仓库内所有资源文件，禁止任何公众号、自媒体进行任何形式的转载、发布。
- 该项目的归属者对任何脚本问题概不负责，包括但不限于由任何脚本错误导致的任何损失或损害。
- 间接使用脚本的任何用户，包括但不限于建立 VPS 或在某些行为违反国家/地区法律或相关法规的情况下进行传播, 该项目的归属者对于由此引起的任何隐私泄漏或其他后果概不负责。
- 如果任何单位或个人认为该项目的脚本可能涉嫌侵犯其权利，则应及时通知并提供身份证明，所有权证明，我们将在收到认证文件后删除相关脚本。
- 任何以任何方式查看此项目的人或直接或间接使用该 Python 项目的任何脚本的使用者都应仔细阅读此声明。 该项目的归属者保留随时更改或补充此免责声明的权利。一旦使用并复制了任何相关脚本或 Python 项目的规则，则视为您已接受此免责声明。

---

[![](https://komarev.com/ghpvc/?username=BNDou&&label=Views "To Github")](https://github.com/BNDou/)
