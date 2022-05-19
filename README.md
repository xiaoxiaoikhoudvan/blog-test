# js对象基本用法

## 1.声明对象的两种语法

* 写法1
```
let obj = {'name':'mike','age':18}
```
* 写法2
```
let obj = new Object({'name':'mike'})
```
* 细节
键名是字符串，不是标识符，可以包含任意字符。
引号可省略，省略之后就只能写标识符。
就算引号省略了，键名也还是字符串。 

## 2. 删除属性
```
delete obj.xxx 或 delete obj['xxx']
```
即可删除obj的xxx属性
注意区分属性值为undefined和不含属性名

# 3. 查看属性
* 查看自身所有属性
```
Object.keys(obj)
```
* 查看自身+共有属性
```
console.dir(obj)
```
* 判断一个属性是自身的还是共有的
```
obj.hasOwnProperty('toString')
```

# 4. 修改或增加对象的属性
* 直接赋值
```
let obj = {name:'mike'}
obj.name = 'xiaohong'
obj['name'] = 'xiaohong'
let key = 'name'
obj[key] = 'xiaohong'
```

* 批量赋值
```
Object.assign(obj,{age:19,gender:'man'})
```

# 5.'name' in obj和obj.hasOwnProperty('name') 的区别

都是两种查看属性是不是在对象里的方法
前者自身属性和共有属性都返回true，后者仅仅是自身属性才返回true


