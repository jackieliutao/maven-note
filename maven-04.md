## Maven核心概念
### 一、Maven坐标
#### 1、什么是坐标？

> 在平面几何中坐标（x,y）可以标识平面中唯一的一个点。

#### 2、Maven坐标主要组成
- groupId：&nbsp;&nbsp;&nbsp;&nbsp;组织标识（包名）
- artifactId：&nbsp;&nbsp;&nbsp;&nbsp;项目名称
- version：&nbsp;&nbsp;&nbsp;&nbsp;项目的当前版本
- packaging：&nbsp;&nbsp;&nbsp;&nbsp;项目的打包方式，最为常见的是<font color='red'><b>jar</b></font>和<font color='red'><b>war</b></font>

> &nbsp;&nbsp;&nbsp;&nbsp;<font color='red'><b>样例：</b></font>

```
      <groupId>com.mycompany.app</groupId>
      <artifactId>myapp</artifactId>
      <version>1.0-SNAPSHOT</version>
      <packaging>jar</packaging>
```
```
      <groupId>com.mycompany.app</groupId>
      <artifactId>myWebApp</artifactId>
      <packaging>war</packaging>
      <version>1.0-SNAPSHOT</version>
```

#### 3、Maven为什么使用坐标？

> &nbsp;&nbsp;&nbsp;&nbsp;Maven拥有大量的构建，需要找一个用来唯一标识一个构建的同意规范

> &nbsp;&nbsp;&nbsp;&nbsp;拥有了统一的规范，就可以把查找工作交给机器

### 二、依赖管理
#### 1、依赖配置

> 依赖配置主要包含如下元素：

```
<!--添加依赖配置-->
<font color='#5400FF'><</font><font color='#800000'>dependencies</font><font color='#5400FF'>></font>
    <font color='#5400FF'><</font><font color='#800000'>dependency</font><font color='#5400FF'>></font>
        <font color='#5400FF'><</font><font color='#800000'>groupId</font><font color='#5400FF'>></font>junit
        <font color='#5400FF'></</font><font color='#800000'>groupId</font><font color='#5400FF'>></font>
```
