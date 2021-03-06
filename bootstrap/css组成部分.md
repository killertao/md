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

```scss
$container-max-widths: (
  sm: 540px,
  md: 720px,
  lg: 960px,
  xl: 1140px,
  xxl: 1320px
); 	
```



#### z-index

```
$zindex-dropdown:                   1000;
$zindex-sticky:                     1020;
$zindex-fixed:                      1030;
$zindex-modal-backdrop:             1040;
$zindex-offcanvas:                  1050;
$zindex-modal:                      1060;
$zindex-popover:                    1070;
$zindex-tooltip:                    1080;
```



#### gird system

> **Sass variables, maps, and mixins power the grid.**  又 变量 maps mixins 为gird 提供动力帮助···``

```scss
.row {
    --bs-gutter-x: 1.5rem;
    --bs-gutter-y: 0;
    display: flex;
    flex-wrap: wrap;
    margin-top: calc(var(--bs-gutter-y) * -1);-gy
    margin-right: calc(var(--bs-gutter-x) / -2);-0.75rem
    margin-left: calc(var(--bs-gutter-x) / -2);-0.75rem
}
.row > * {
    flex-shrink: 0;
    width: 100%;
    max-width: 100%;
    padding-right: calc(var(--bs-gutter-x) / 2);
    padding-left: calc(var(--bs-gutter-x) / 2);
    margin-top: var(--bs-gutter-y);
}
.col-{1-12} {
    flex: 0 0 auto;
    flex-grow: 0;
    flex-shrink: 0;
    flex-basis: auto;
    width: number/12;
}

$grid-gutter-width: 1.5rem;
$gutters: (
  0: 0,
  1: $spacer * .25,
  2: $spacer * .5,
  3: $spacer,
  4: $spacer * 1.5,
  5: $spacer * 3,
);
```



### Utilities

#### display

```scss
 "display": (
      responsive: true,
      print: true,
      property: display,
      class: d,
      values: inline inline-block block grid table table-row table-cell flex inline-flex none
    ),
eg:
d-flex
d-block 
d-md-flex,d-sm-block
```

#### flex

~~~scss
.d-flex
.flex-{direction} row,column,rowreverse,columnreverse

.just-content-{flex-layout} start,end center between space-around
.align-items-{flex-layout}
.align-content-{flex-layout}
.flex-wrap :warp|nowrap|wrapreverse
.flex-fill{
    flex-flow:1 1 auto
}
.flex-grow-[0,1]
.flex-shrink-[0,1]
.flex-order-[first,0-5,last],

~~~



#### spacing

```scss
$spacers: (
  0: 0,
  1: $spacer / 4,
  2: $spacer / 2,
  3: $spacer,
  4: $spacer * 1.5,
  5: $spacer * 3,
) !default;

{property}{sides}-{size} 
{property}{sides}-{breakpoint}-{size}
property(
	m:'margin',
    p:'padding'
)
sides(
    t:"top",
    b:"bottom",
    s:"start left",
    e:"end right",
    x:'s|e',
    y:'b|t',
    '':"没有的话就是4个边"
)
size(
    0 - for classes that eliminate the margin or padding by setting it to 0
    1 - (by default) for classes that set the margin or padding to $spacer * .25
    2 - (by default) for classes that set the margin or padding to $spacer * .5
    3 - (by default) for classes that set the margin or padding to $spacer
    4 - (by default) for classes that set the margin or padding to $spacer * 1.5
    5 - (by default) for classes that set the margin or padding to $spacer * 3
    auto - for classes that set the margin to auto
)
eg:mt-0,mx-0,m-auto,m-t-sm-auto
```

#### borders



#### sizing



#### background



#### colors

#### 

#### position

#### float 

#### text

#### vertical align

#### visibility

#### shadows

#### overflows

#### Interactions

