基于此日历基础上增加以下功能

## 1:日历左右滑动,更符合移动端操作

  由于已经修改了原文件,所以不适合添加插件的方式添加.添加方式
  
  1.1 将plugin\components\calendar目录copy到自己项目目录
  
  1.2 添加引用,(原生小程序在json里面添加,wepy在config中添加)
  
     "usingComponents": {
        "calendar": "../plugin/components/calendar"
      }
      
  1.3 其他用法与原插件一致
  1.4 解决首行日期和未行日期cell对齐的bug
## 2:自定义日期样式

  原有的配置只适合设置背景和字体颜色,实际情况中可能需要用到图片背景或者圆框,所以在这里添加了日期Day Cell的css样式;
  
  使用方法与原来的样式设定类似,添加了className属性,指向自己设定的css,注意这个css需要写在calendar.wxss里面
  
  如:
  
  
  ```
  .calendar-cell-customerCss{
     border: 1px solid #0BB20C;
    }
  ```
  
  样式设定
  
  ```
  this.days_style.push({ month: 'current', day: 12, color: 'white', background: '#CD4737', className:'calendar-cell-customerCss'});
  ```

## 微信小程序「极点日历」插件

「极点日历」插件支持 1900 年 1 月 ~ 2099 年 12 月这两百年间的公历和农历显示，插件提供了丰富的可配置属性，包括日期的显示方式、选择范围、是否显示农历等，可自定义来适配不同的使用场景。

插件ID：wx92c68dae5a8bb046

版本历史：

v1.0.0 完成插件基本功能

v1.1.0 修复日期点击bug

具体的使用方法，可以参考下面的接口文档和用法例子

1、[添加插件到自己的小程序](https://github.com/czcaiwj/calendar/wiki/%E6%B7%BB%E5%8A%A0%E6%8F%92%E4%BB%B6%E5%88%B0%E8%87%AA%E5%B7%B1%E7%9A%84%E5%B0%8F%E7%A8%8B%E5%BA%8F)

2、[日历属性接口文档](https://github.com/czcaiwj/calendar/wiki/%E6%97%A5%E5%8E%86%E5%B1%9E%E6%80%A7%E6%8E%A5%E5%8F%A3%E6%96%87%E6%A1%A3)

3、[日历事件用法](https://github.com/czcaiwj/calendar/wiki/%E6%97%A5%E5%8E%86%E4%BA%8B%E4%BB%B6%E7%94%A8%E6%B3%95)

4、[自定义日历样式](https://github.com/czcaiwj/calendar/wiki/自定义日历样式)

## 插件使用效果演示

Demo1

![Demo1](http://imcoding.org/Public/resource/img/calendar/demo1.jpg)

Demo2

![Demo2](http://imcoding.org/Public/resource/img/calendar/demo2.jpg)

Demo3

![Demo3](http://imcoding.org/Public/resource/img/calendar/demo3.jpg)

Demo4

![Demo4](http://imcoding.org/Public/resource/img/calendar/demo4.jpg)

Demo5

![Demo5](http://imcoding.org/Public/resource/img/calendar/demo5.jpg)

Demo6

![Demo6](http://imcoding.org/Public/resource/img/calendar/demo6.jpg)

Demo7

![Demo7](http://imcoding.org/Public/resource/img/calendar/demo7.jpg)
