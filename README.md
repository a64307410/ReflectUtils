# ReflectUtils

简化java反射调用方式，用来获取属性、调用方法以及做一些判断（是否为公共的、私有的...）

[具体文档请点击](https://baonanhai.github.io/ReflectUtils/)

使用样例

#### 1、获取属性
```java
ReflectUtils.getField(TestClass.class, "field1");
```

#### 2、获取成员属性值
```java
ReflectUtils.getFieldValue(new TestClass(), "field1");
```

#### 3、获取类静态属性值
```java
ReflectUtils.getStaticFieldValue(TestClass.class, "field2");
```

#### 4、设置属性值
```java
ReflectUtils.setFieldValue(new TestClass(), "field1", "eee");
```

#### 5、设置类静态属性值
```java
ReflectUtils.setStaticFieldValue(TestClass.class, "field2", "fff");
```

#### 6、获取方法
```java
ReflectUtils.getMethod(TestClass.class, "append", String.class, String.class);
```

#### 7、执行方法
```java
ReflectUtils.invokeMethod(new TestClass(), "append1", "xxx");
```

#### 8、执行静态方法
```
ReflectUtils.invokeStaticMethod(TestClass.class, "append", "xxx", "ttt");
```
有BUG或者建议请联系baonanhai@gmail.com
