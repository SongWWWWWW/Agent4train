[//]: # (# Agent4travel)

[//]: # (> [!IMPORTANT])

[//]: # (> **重大更新：**)

[//]: # (> 2024/8/14: 更新内容)

[//]: # (> 1. 将agent，backend，frontend，Model，tools部分分开)

[//]: # (> 2. 将所有配置全部集中在配置文件)

[//]: # (> 3. 将agent流程分开，分为SuperAgent和ToolsAgent，重写对话流程)

[//]: # (> 4. 将模型问答，baidu api 调用放置到后端api中)

[//]: # (> 2024/8/20: 更新内容)

[//]: # (> 1. 添加tool, 多地点路线规划，景点图片查询，某地景点查询)

[//]: # (> 2. 添加图片展示)

[//]: # (> 3. 添加后端api)

# Agent4travel

> [!IMPORTANT]
> **重大更新：**
>
> **2024/8/14 更新内容:**
> 1. 将 `agent`、`backend`、`frontend`、`Model`、`tools` 部分分开，模块化结构更清晰。
> 2. 将所有配置集中到配置文件中，方便管理和修改。
> 3. 将 `agent` 流程分为 `SuperAgent` 和 `ToolsAgent`，并重写了对话流程，提高了系统的灵活性和可扩展性。
> 4. 将模型问答和百度 API 调用功能整合到后端 API 中，简化前端调用流程。
>
> **2024/8/20 更新内容:**
> 1. 新增工具:
>    - 多地点路线规划。
>    - 景点图片查询。
>    - 某地景点查询。
> 2. 添加图片展示功能，提升用户体验。
> 3. 扩展了后端 API 的功能，增强了系统的整体性能和功能性。
>
> **2024/8/24 更新内容:**
> 1. 新增yuan模型支持
> 
> 

### 按照下面这个步骤进行环境配置
```bash
conda create -n agent4train python=3.12
conda activate agent4train
pip install -r requirements.txt
```
```bash
# 请将config.toml.temp更名为config.toml,并将环境变量填入
#启动👇
python backend/api.py # 启动后端
streamlit run main.py # 启动前端
```
### 效果展示
[示例视频](https://github.com/SongWWWWWW/Agent4train/blob/master/video.mp4)