<p align="center">
  <a href="http://ant.design">
    <img width="520" src="http://git.onemt.com.cn/tongxiang/onemt-loading/raw/develop/static/image/logo.png">
  </a>
</p>

# Onemt-loading 共用loading加载页面

## 概述:

onemt-loading 是一套根据公司不同的后台系统开发的基础样式库，可以令用户的使用感知更加统一。样式中对背景色以及icon动画颜色都可以进行配置。

## 颜色配置:
现有的颜色配置为以下配色，后续可根据需求另行添加；
<p align="left">
    <img width="820" src="https://raw.githubusercontent.com/UEDNewbie/onemt-loading/develop/static/image/theme-color.jpg">
</p>

- .skin-red [ #BD3232 ]

- .skin-orange [ #FE9A76 ]

- .skin-yellow [ #FFD700 ]

- .skin-green [ #016936 ]

- .skin-blue [ #0E6EB8 ]

- .skin-grey [ #afafaf ]

- .skin-black [ #000000 ]

- .skin-white [ #ffffff ]

## 项目下载:

```
git clone http://tongxiang@git.onemt.com.cn/tongxiang/onemt-loading.git

运行 index.html 即可预览效果

```
## 引用:

--非jsx引用
```
<link href="static/css/index.css" rel="stylesheet">
```
--jsx引用
```
import Loading from './loading';

 <Loading />
```
此时要将js文件下对应目录的loading.js文件放在common文件夹下，并将scss文件夹下文件copy进去,并在index.scss中`@import './loading';`
```
├── static                                        
│   ├── js                              
│   │   ├── controller                             
│   │   │   ├── component 
│   │   │   │   ├── common 
│   │   │   │   │  ├── loading.js 
│   ├── scss
│   │   ├── assert
│   │   ├── _loading.scss     
│   │   ├── _theme.scss    
```

## 使用方法:
  `skin-颜色` 即背景色，icon颜色默认为白色，只有`skin-white`背景色为白色时，icon颜色为公司logo原色橘黄色；
  
  `skin-颜色-Num` 即可以给背景色加透明度，icon透明度不变；
  
  >> 背景无透明度
```
  <div class="loading skin-white">
    <div class="loading-con">
      ...
        <span></span>
    </div>
  </div>
```
  >> 背景有透明度
```
  <div class="loading skin-white-3">
    <div class="loading-con">
      ...
        <span></span>
    </div>
  </div>
```
#### jsx语法中只需要将`class`换成`className`即可；
  
## 贡献:

如果你有好的意见或建议，欢迎给我们提issue或pull request，为提升loading体验贡献力量
