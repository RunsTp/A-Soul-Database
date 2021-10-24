### 半自动字幕生成器

##### 剪映的语音识别接口通过抖音的万亿级数据使他的准确度和速度都不错,而且免费。但并不开放接口，对于多视频而言并不友好，该工具使用<b>Pyautogui 点击库来帮助构建一个简单的字母转换工具

###### 使用
1.执行`pip install -r requirements` 安装库
2.配置 `config.json`
```
draftContentPath 剪映的工作目录
videoDir 视频的存放目录
theme Windows的主题(Light:浅色,Dark:深色)务必遵循大小写
confidence 对比置信度，实测0.6时效果尚可
```
3. `python main.py`
因为剪映无法及时释放文件锁，故运行完毕之后只会弹出已完成的视频文件名,请手动进行下一步操作