![](brand-colors.png)

brand-colors 是一个品牌颜色合集，可用于sass，less，stylus和css中。

## 安装

```
npm install brand-colors
bower install brand-colors
```

## 用法

#### scss
```scss
@import 'bower_components/brand-colors/dist/latest/scss/brand-colors.latest.scss'

.a-div {
  color: $bc-spotify;
}
```
#### less
```css
@import 'bower_components/brand-colors/dist/latest/less/brand-colors.latest.less'

.a-div {
  color: @bc-spotify;
}
```
##### 在webpack中
  * 使用相對路徑 `node_modules`, 比如:
  
  ```js
    app
     |_node_modules
     |_src
        |_css
           |_app.less
  ```
  in app.less:
  
  ```less
  @import '../../node_modules/brand-colors/dist/latest/less/brand-colors.latest.less';
  ```
  
  * use webpack's resolve mechanism
  
  ```less
  @import '~brand-colors/dist/latest/less/brand-colors.latest.less';
  ```
  
#### sass
```sass
@import 'bower_components/brand-colors/dist/latest/scss/brand-colors.latest.sass'

.a-div
  color: $bc-spotify
```
#### stylus
```css
@import 'bower_components/brand-colors/dist/latest/stylus/brand-colors.latest.styl'

.a-div {
  color: $bc-spotify;
}
```
#### css

```html
  <link rel="stylesheet" href="bower_components/brand-colors/dist/latest/css/brand-colors.latest.min.css">`

  <span class="bc-spotify">This text is spotify-green</span>
  <div class="bc-spotify-bg">This div has a spotify-green background</div>
```
#### postcss

Use [postcss-brand-color](https://github.com/postcss/postcss-brand-colors) plugin. Add it to PostCSS:

```js
postcss([ require('postcss-brand-colors') ])
```

并使用颜色名 `*-color`:

```css
.a-div {
  color: spotify-color;
}
```

### 在本地运行brand-colors.com
如果您想对静态网页的工作，只需要运行下面的命令
你会得到一个活重装服务器监听在/ app变化
and brandColors.js
```bash
npm install
gulp dev
```
### Brands
[Full list of colors](https://github.com/reimertz/brand-colors/blob/master/data/brandColors.js#L8)
A lot fo the colors comes from brandcolors.net, so a huge shout out to @galengidman.

---
> [reimertz.co](http://reimertz.co) &nbsp;&middot;&nbsp;
> GitHub [@reimertz](https://github.com/reimertz) &nbsp;&middot;&nbsp;
> Twitter [@reimertz](https://twitter.com/reimertz)
