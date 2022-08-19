# zhenxunbot_GPT-2
本项目受到早苗bot启发，且无法忍受青客云屑AI，因此在GitHub上寻找代替方案  
使用前请先安装运行库：
```
pip install -r requirements.txt -i https://pypi.douban.com/simple
```

## 本项目由[yangjianxin1](https://github.com/yangjianxin1)大佬的[GPT2-chitchat](https://github.com/yangjianxin1/GPT2-chitchat)项目修改（如有侵权联系删除）
仅在原项目上增加使用Flask库进行网页交互，几乎照抄  

***仅使用cpu进行对话生成，由于闲聊对话生成的内容长度不是很长，因此生成部分在CPU上跑速度也挺快的***

<h2 id="model_share">模型分享</h2>

|模型 | 共享地址 |模型描述|
|---------|--------|--------|
|model_epoch40_50w | [百度网盘【提取码:ju6m】](https://pan.baidu.com/s/1iEu_-Avy-JTRsO4aJNiRiA) 或 [GoogleDrive](https://drive.google.com/drive/folders/1fJ6VuBp4wA1LSMpZgpe7Hgm9dbZT5bHS?usp=sharing) |使用50w多轮对话语料训练了40个epoch，loss降到2.0左右。|

将下载好的模型放入model/model_epoch40_50w文件夹中即可  
如需训练自己的GPT-2模型详见[原项目](https://github.com/yangjianxin1/GPT2-chitchat)  

### 默认使用本地5000端口，并使用get请求  
例如：
```
http://127.0.0.1:5000/?key_word=我喜欢你
答：我也喜欢你
```
