# HTML常用标签

## 一、a 标签
a元素（或称锚元素）可以通过它的 href 属性创建通向其他网页、文件、同一页面内的位置、电子邮件地址或任何其他 URL 的超链接。a 中的内容应该应该指明链接的意图。如果存在 href 属性，当 a 元素聚焦时按下回车键就会激活它。

代码示例：
```
<p>You can reach Michael at:</p>

<ul>
  <li><a href="https://example.com">Website</a></li>
  <li><a href="mailto:m.bluth@example.com">Email</a></li>
  <li><a href="tel:+123456789">Phone</a></li>
</ul>
```

## 二、img 标签

img 元素将一份图像嵌入文档

代码示例：
```
<img class="fit-picture"
     src="/media/cc0-images/grapefruit-slice-332-332.jpg"
     alt="Grapefruit slice atop a pile of other slices">
```
## 三、table 标签

table 元素表示表格数据 — 即通过二维数据表表示的信息

代码示例：
```
<table>
    <thead>
        <tr>
            <th colspan="2">The table header</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>The table body</td>
            <td>with two columns</td>
        </tr>
    </tbody>
</table>
```

