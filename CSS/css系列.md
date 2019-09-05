
### CSS3

* border-radius // 圆角 （最多八个值，前四个和后四个中间用“/”线分隔）

* box-shadow // 盒阴影 (inset 20px 20px 30px blue)

* text-shadow // 字阴影 （当需要添加多个阴影的时候，中间用','分隔，box-shadow一样）

* background-size // 设置背景图片大小（contain / cover）

* background-origin // 设置背景图原点 (border-box / padding-box / content-box)

* background-clip // 设置背景图的裁剪

* 线性渐变
 background: linear-gradient() // 线性渐变 (to right, red, blue) (45deg, red, blue)

```
        div{
            width: 200px;
            height: 200px;
            background: linear-gradient(45deg,red 30%,lightskyblue,blue);
        }

    <div></div>
```

![线性渐变](http://upload-images.jianshu.io/upload_images/2941543-e5621b2f2229fa2f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
> 百分比写不写都行

* 径向渐变
background: radial-gradient() // 径向渐变 (at 100px 100px, red, blue)
```
        div{
            width: 200px;
            height: 200px;
            background: radial-gradient(at  50px 50px,red 10%,blue,gold)
        }

    <div></div>
```

![径向渐变 他在发呆](http://upload-images.jianshu.io/upload_images/2941543-7954f24c37681418.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)



### CSS4

* 否定伪类:not

**eg：**

```
p:not(.intro) {}

在CSS4选择器中，可以传入一个逗号(,)分隔的列表选择器：

p:not(.intro, blockquote) {}
```

* 匹配任何伪类:matches

```
p:matches(.alert, .error, .warn) { color: red; }

带有只要元素带<p>带有.alert、.error和.warn中任何一个类名，文本颜色都将会是red。
```

* 关系伪类:has

```
a:has( > img ) { border: 1px solid #000; }
// 任何一个包含<img>的<a>链接都会加上一个黑色的边框

li:not(:has(p)){}
// 不包含段落<p>的<li>元素
```

* 表单限制伪类 :required：optional

```
匹配表单项中必选项与可选项。
input:required { color:#f30; }
```

* 可读可写伪类 :read-write、:read-only

* :any-link

```
它会检查href的是否在用户的浏览历史中存在，以确定是否一个给定的链接是否已被访问。

:link, :visited {

color: blue;

}

css4 ，可以直接这样应用，上述代码等价于：

:any-link {

color: blue;

}
```

* scoped,仅当前文件样式使用

```
<style scoped>
```

* 网格布局

















