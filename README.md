### 加form标签的好处
	1. 可以使用submit reset等标签，
    2. 部分框架可以使用form批量获取表单数据
    3. 用户体验方面，浏览器可以弹出是否保存用户和密码
    4. 第三方库可以进行表单验证

### html5新增语义
需要在日常开发中养成好习惯，多使用有语义的标签
	- header/footer 头尾
	- section/article 区域
	- nav   导航
	- aside 不重要内容
	- em/strong 强调

### 层叠样式表CSS

#### 浏览器解析CSS选择器的顺序
从右往左的方式，比如
```css
.body div a{
	color:red
}
```
会先找到a标签判断它的父亲是否为div，父亲的父亲是否含有.body选择器

#### 选择器的分类
	- 元素选择器
    - 伪元素选择器 ::before
    - 类选择器
    - 属性选择器 [type=radio]{}
    - 伪类选择器
    - id选择器
    - 组合选择器 [type=checkbox] + label{}
    - 否定选择器 :not(.link){}
    - 通用选择器

#### 文字的对齐

一般的文字默认使用基线对齐 vertical-align: baseline;
一般的居中对齐使用 vertical-align: middle;
也可以使用顶线对齐 top或底线bottom
#### 解决行内图片末尾缝隙的问题
行内的图片默认遵从baseline基线对齐，所以默认会和低有一定的空隙，这是使用底线对齐就可以解决该问题

#### 使用背景色叠加实现网格

```css
<style>
div{
    height: 60px;
    background: linear-gradient(135deg, transparent 0, transparent 49.5%, red 50%, transparent 50.5%, transparent 100%),
       		    linear-gradient(45deg, transparent 0, transparent 49.5%, green 50%, transparent 50.5%, transparent 100%);
    background-size: 30px 30px;
}
</style>
```

#### base64压缩的优缺点
- 减少了http请求
- 文件会增大
- 服务器需要解码，
- 适用于小图标





















