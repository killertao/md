### css组成部分

```
Layout 布局 
Content 内容部分
Components 组件部分
Utilities 部分 
```

### 文件组成部分

```
bootstrap-reboot.css Content部分，对格式浏览器进行样式重置和统一 
bootstrap-grid.css 	 Layout Grid System grid 栅栏布局 ,Utilities 帮助类 
bootstrap.css	 4个部分都包含
```

### 页面布局

#### breakpoints 

```scss
$grid-breakpoints: (
  xs: 0,
  sm: 576px,
  md: 768px,
  lg: 992px,
  xl: 1200px,
  xxl: 1400px
);
```



#### container

```
.container: 设置了最大宽度 在每个屏幕尺寸下
.container-fulid 100% 所有屏幕尺寸
.container-{break-point}  知道指定尺寸，宽度都是100%
```



#### z-index

```
$zindex-dropdown:          1000 !default;  下来列表布局
$zindex-sticky:            1020 !default;  sticky 布局
$zindex-fixed:             1030 !default;  fixed 布局
$zindex-modal-backdrop:    1040 !default;  
$zindex-modal:             1050 !default;  modal 弹出框
$zindex-popover:           1060 !default;  popover  页面上层框
$zindex-tooltip:           1070 !default;  tooltip 提示框
```



