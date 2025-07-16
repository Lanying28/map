<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>地图画布 V11.0 - 纯净版</title>
    <style>
        /* 样式简化到极致，确保地图铺满全屏 */
        html, body, #map-container {
            margin: 0;
            padding: 0;
            width: 100%;
            height: 100%;
        }
    </style>
    <script charset="utf-8" src="https://map.qq.com/api/gljs?v=1.exp&key=AQDBZ-ZRTOJ-XJ7FG-XRSWJ-56UU2-RTBS5"></script>
</head>
<body>

<div id="map-container"></div>

<script>
    // 页面加载后只做一件事：初始化一张干净的地图
    window.onload = function() {
        
        // 初始化地图，设定一个宏观的初始视角
        const map = new TMap.Map(document.getElementById('map-container'), {
            center: new TMap.LatLng(34.75, 103.75), // 中国大陆地理中心的大致位置
            zoom: 5,           // 一个适合观察全国的缩放级别
            pitch: 0,          // 零俯仰角，平视地图
            rotation: 0        // 零旋转角，正北朝上
        });

        // 所有关于标记、图例、信息窗体的代码均已移除。
    }
</script>

</body>
</html>
