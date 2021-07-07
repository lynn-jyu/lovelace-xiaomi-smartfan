# Xiaomi Fan Lovelace Card
[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg)](https://github.com/custom-components/hacs)

Xiaomi Pedestal Fan Lovelace card for HASS/Home Assistant.

Only for dmaker.fan.p8.

+  Supports [HACS](https://github.com/custom-components/hacs) installation
+  Works seamlessly with the [syssi/xiaomi_fan](https://github.com/syssi/xiaomi_fan) integration
+  Animations of the fan are made purely with CSS
+  Hold to adjust fan speed 
+  ~~Hold to adjust oscillating angle (30, 60, 90, 120, 140) degrees~ (Not supported on Pedestal Fan P8)
+  Translation for titles

## HACS Installation
1. Navigate to HACS 
1. Choose "Frontend"
1. Choose "Custom repositories" from the top right button
1. Enter "https://github.com/lynn-jyu/lovelace-xiaomi-smartfan" in "Add custom repository URL", Choose "Lovelace" for "Category"
1. Find "Xiaomi smartfan Card (Pedestal Fan P8)"  in "Frontend" and click "Install"


## Manual Installation
1. Download `smartfan-xiaomi.js`
1. Copy to `www/plugins/lovelace-xiaomi-smartfan/xiaomi-smartfan.js`
1. Add the following to your Lovelace resources
    ``` yaml
    resources:
    - url: /local/lovelace-xiaomi-smartfan/xiaomi-smartfan.js
      type: js
    ```
1. Add the following to your Lovelace config `views.cards` key
    ```yaml
    - entity: fan.entity_id
      name: Fan Name
      type: 'custom:smartfan-xiaomi'
      translate: #optional for titles in any language
        Angle: 
        Child Lock:
        Natrual:
        Off:
        On:
        Oscillate:
        Speed Level:
        Timer:
    ```
    Replace `fan.entity_id` with your fan's entity_id and `Fan Name` with any name you'd like to name your fan with
    
    

# 小米落地扇(交流电版) lovelace卡片
[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg)](https://github.com/custom-components/hacs)

HA 小米落地扇(交流电版) lovelace 卡片

仅支持dmaker.fan.p8

+  支持 [HACS](https://github.com/custom-components/hacs) 
+  配合 [syssi/xiaomi_fan](https://github.com/syssi/xiaomi_fan) 使用
+  纯CSS 动画效果
+  长按风速按钮调整风扇速度
+  ~~长按摆风按钮调整摆风角度(30, 60, 90, 120, 140)度~(米家落地扇P8不支持)
+  支持文本多语言

## HACS 安装
1. 打开HACS 
1. 选择“前端”
1. 右上角下拉菜单选择“自定义存储库”
1. “添加自定义存储库URL“ 输入 "https://github.com/lynn-jyu/lovelace-xiaomi-smartfan" , “类别”选择“ "Lovelace" 
1. 在前端页面找到 "Xiaomi smartfan Card (Pedestal Fan P8)"  点击 “安装”

## Manual Installation
1. 下载 `smartfan-xiaomi.js`
1. 拷贝 到 `www/plugins/lovelace-xiaomi-smartfan/xiaomi-smartfan.js`
1. 在lovelace资源添加
    ``` yaml
    resources:
    - url: /local/lovelace-xiaomi-smartfan/xiaomi-smartfan.js
      type: js
    ```
1. 在视图卡片内添加
    ```yaml
    - entity: fan.entity_id
      name: Fan Name
      type: 'custom:smartfan-xiaomi'
      translate: #optional for titles in any language
        Angle: 
        Child Lock:
        Natrual:
        Off:
        On:
        Oscillate:
        Speed Level:
        Timer:
    ```
    替换实际的设备id `fan.entity_id`  修改名称`Fan Name`  
    
## Credits
[fineemb](https://github.com/fineemb) (Original author)

[ikaruswill](https://github.com/ikaruswill/) 

[iwzoo](https://github.com/iwzoo/) (forked from)

[shaonianzhentan](https://github.com/shaonianzhentan/)

[花神](https://github.com/yaming116)
