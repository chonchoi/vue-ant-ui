## Badge 徽标数

图标右上角的圆形徽标数字。

## 何时使用

一般出现在通知图标或头像的右上角，用于显示需要处理的消息条数，通过醒目视觉形式吸引用户处理。

## 代码演示

<demo></demo>

<script>
import Demo from 'pages/badge/demo'

export default {
  components: {
    Demo
  }
}
</script>

## API

```
<ant-badge :count="5">
  <a href="#" class="head-example" />
</ant-badge>
```


```
<ant-badge :count="5" />
```

| 参数           | 说明                             | 类型       |  可选值 | 默认值 |
|----------------|----------------------------------|------------|---------|--------|
| count          | 展示的数字，大于 overflowCount 时显示为 `${overflowCount}+`，为 0 时隐藏 | Number     |         |        |
| overflowCount  | 展示封顶的数字值                 | Number     |         | 99     |
| dot            | 不展示数字，只有一个小红点       | Boolean    |         | false  |
| status         | 设置 Badge 为状态点            | Enum      | 'success'、'processing'、'default'、'error'、'warning' | '' |
| text           | 在设置了 `status` 的前提下有效，设置状态点的文本  | String | | '' |