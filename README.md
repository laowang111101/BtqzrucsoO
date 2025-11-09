# 前言

蜀味道江湖餐饮管理系统是一款基于Java语言和Spring Boot框架开发的餐饮管理系统小程序。该系统结合了JS、Vue和CSS3前端技术，采用MySQL数据库进行数据存储，致力于为餐饮行业提供便捷、高效的管理解决方案。以下是该项目的基本介绍。

## 内容介绍

本项目主要包括以下功能模块：用户模块、菜品模块、订单模块、管理员模块等。用户模块提供用户注册、登录、查看菜单、下单等功能；菜品模块负责菜品的展示、分类和搜索；订单模块处理订单的生成、支付和状态跟踪；管理员模块则负责对用户、菜品、订单等进行管理。通过这些模块的协同工作，餐饮企业可以轻松实现线上线下业务的整合。

## 技术介绍

- 语言：Java
- 使用框架：Spring Boot
- 前端技术：JS、Vue、CSS3
- 开发工具：IDEA/Eclipse
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven: apache-maven 3.8.1-bin
- 前端环境：Node.Js 12\14\16

## 核心代码

以下是项目中的一部分核心代码：

```java
// 获取菜品列表
@GetMapping("/dish/list")
public R<List<Dish>> list(@RequestParam("categoryId") Long categoryId,
                          @RequestParam(value = "status", required = false) Integer status) {
    LambdaQueryWrapper<Dish> queryWrapper = new LambdaQueryWrapper<>();
    queryWrapper.eq(Dish::getCategoryId, categoryId);

    if (status != null) {
        queryWrapper.eq(Dish::getStatus, status);
    }

    List<Dish> list = dishService.list(queryWrapper);
    return R.success(list);
}
```

## 免费源码获取

```
8000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img13.360buyimg.com/ddimg/e20004)

![介绍图片](https://img14.360buyimg.com/ddimg/e20004)

![介绍图片](https://img11.360buyimg.com/ddimg/e20004)

![介绍图片](https://img14.360buyimg.com/ddimg/e20004)

![介绍图片](https://img13.360buyimg.com/ddimg/e20004)

![介绍图片](https://img14.360buyimg.com/ddimg/e20004)

![介绍图片](https://img10.360buyimg.com/ddimg/e20004)

![介绍图片](https://img11.360buyimg.com/ddimg/e20004)

![介绍图片](https://img10.360buyimg.com/ddimg/e20004)

![介绍图片](https://img13.360buyimg.com/ddimg/e20004)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
