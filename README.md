# JS 函数的执行时机

## 1. 解释为什么如下代码会打印 6 个 6
```
let i = 0
for(i = 0; i<6; i++){
  setTimeout(()=>{
    console.log(i)
  },0)
}
```
答： 因为是先把for执行完，此时i=6，然后再执行打印，所以是打印出6个6

## 2. 写出让上面代码打印 0、1、2、3、4、5 的方法

```
for (let i = 0; i < 6; i++) {
    setTimeout(() => {
        console.log(i);
  }, 0);
}
```

