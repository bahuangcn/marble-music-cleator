# Marble Music Creator

这是一个辅助插件，用于简化在 Blender 中创建弹珠音乐视频的工作。

<img src="https://github.com/user-attachments/assets/b6e0437a-ccae-4095-9230-8d14fd006224" width="25%">
<img src="https://github.com/user-attachments/assets/c3367b84-ea5c-4c0a-b252-01764403ffb9" width="25%">

## 使用方法

<img src="https://github.com/user-attachments/assets/c54ad029-0256-4898-8776-bde64a3a4b6c" width="50%">

请将 marble_music_creator.py 作为 Blender 插件安装。  
视口侧边栏中会添加 Marble Music Creator 面板。

**Target Object**　- 请选择球体对象。  
**Prefab Object** - 请选择板子对象。  
**Collection Of Instance** - 请选择放置复制对象的集合。（如果不选，则与复制源使用同一集合。）  
**Position Offset** - 决定板子放置在距离球体多远的位置。请设置为略大于球体半径的值。  
**Random Rotation Angle** - 决定板子相对于球体行进方向倾斜角度的最大值。

请为球体和板子设置刚体。  
请将音乐文件放入序列编辑器。  
在播放时间线的同时，配合音乐按下 **Duplicate Prefab** 按钮。  
每次按下按钮，都会在球体的前进方向上放置一块板子，球体会弹跳。

## 示例

请参考 sample 文件夹中的 blend 文件。

## 已知问题

- 球体有时会碰到之前放置的板子
  - 这是因为板子的角度是纯随机的，完全没有考虑球体之前的轨迹。  
    请手动调整板子角度来解决。
