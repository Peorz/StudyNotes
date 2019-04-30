# Kotlin笔记

## 最基础语法

### 主函数
```
fun main() {
    print("hello kotlin")
}
```

### 定义函数
```
//定义函数的基本格式
fun doSth(){

}
```
```
//定义带参数的函数
fun setName(name : String){
    
}
```
```
//带返回值的函数
fun getName(): String {
    return "xlh"
}
```

### 定义变量
* `var name = "xlh"` 定义变量使用**var**
* `val name = "xlh"` 定义不可变的变量**val**
* `var name : String = "xlh"` 在变量名后用`:`指定类型
* `var name : String? = null` 定义可以为null的变量（String!和String不是同一个类型）

### 模版语法
```
fun main() {
    myPrint("xlh")
}

//在字符串中使用 $ 引用变量
fun myPrint(str:String){
    print("my name is $str")
}
```
