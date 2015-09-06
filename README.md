# TextareaField 多行文本框


## TL;DR

1. 这是一个 tingle 组件，表单多行文本框，包括标题和表单，展示效果如下：  
![效果图](https://gtms03.alicdn.com/tps/i3/TB1wzN5IVXXXXcxaXXXFIRO8VXX-445-198.png_200x200.jpg)

## Simple Usage

```
<TextareaField label="三个字" minRows={2} maxRows={5} 
placeholder="3个行高 最大5个行高" value={t.state.remark}
onChange={t.handleChange.bind(t)}/>
                    
<TextareaField label="只读" value="不能更改" readOnly={true}/>
```

## 可用配置

| 配置项 | 类型 | 默认值 | 功能/备注 |
|---|----|---|----|
|minRows|Interger|1|最小显示行|
|maxRows|Interger|10|最大行，超过则显示滚动条|
|placeholder|String|``|提醒文案，默认空|
|readOnly|Boolean|false|是否只读，只读时不能输入，默认false|
|lineHeight|Interger|22|行高，默认22px|
|onChange|Function| function() {} | 输入内容变化时触发 |
|onFocus|Function| function() {} | 获取到输入焦点时触发 |
|onBlur|Function| function() {} | 与pc端一致，鼠标离开时响应 |

## API 接口

本组件无外部接口可用

## 事件

- onChange(newValue, e) 

````javascript
// 新值和事件对象
handleChange(newValue,e) {
    
}

````

- onFocus(e) 

- onBlur(e) 



## Links 相关链接

- [Fire a bug/Issues 提 Bug](https://github.com/tinglejs/tingle-textarea-field/issues)

- [tingle](https://github.com/tinglejs)



# 如何删除git submodule子项
imouse posted @ 2012年11月11日 03:29 in Linux with tags Git submodule , 1743 阅读
1. 编辑.gitmodules,删除对应要删除的submodule的行．

2. 编辑.git/config,删除有对应要删除的submodule的行．

3. 删除命令:

    git rm --cached bundle/xxxx  (PS:此处最后没有符号 / .)

4. 删除对应的目录:

    rm -rf bundle/xxxx
