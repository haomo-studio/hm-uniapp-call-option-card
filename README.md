> 官网: [https://haomo-tech.com](https://haomo-tech.com)

> 作者: 毫末科技

> 邮箱: hxg@haomo-studio.com

## 预览

![预览图片](http://downloads.haomo-tech.com/uniapp/hm-call-option-card.png)

[在线效果预览](http://template.uniapp.haomo-tech.com/pages/haomo/test-component/hm-call-option-card)

更多毫末科技的uni-app跨端模板，请见[毫末科技uni-app跨端模板](https://haomo-tech.com/sale.html)

## 技术支持

我们公司提供超低价的切图服务哈。移动端平均50元每个页面，PC Web端平均80元每个页面。目前支持出vue、react、uniapp、taro、flutter、小程序代码代码，代码支持自适应。其中uniapp、taro一份代码支持多端。app原生会在五月份开始支持。示例demo: [http://edu.uniapp.haomo-tech.com](http://edu.uniapp.haomo-tech.com)。部分样例代码：[http://downloads.haomo-tech.com/uniapp-demo.zip](http://downloads.haomo-tech.com/uniapp-demo.zip)

* [uni-app插件市场](https://ext.dcloud.net.cn/plugin?id=1564)

* [npm包](https://www.npmjs.com/package/hm-uniapp-call-option-card)

* [github地址](https://github.com/haomo-studio/hm-uniapp-call-option-card)

* [gitee地址](https://gitee.com/haomo/hm-uniapp-call-option-card)

毫末科技将长期迭代本组件。需要技术支持，请进钉钉群（群号30423559）：

<img width="250" src="http://downloads.haomo-tech.com/%E6%AF%AB%E6%9C%ABuniapp%E7%BB%84%E4%BB%B6%E6%8A%80%E6%9C%AF%E6%94%AF%E6%8C%81.jpg">

## 概述

毫末uni-app毫末通话选择卡片组件。支持H5/小程序(微信、支付宝、头条、百度、QQ)/App；组件可自适应各种屏幕大小的手机。

## 使用

请使用HBuilderX导入组件。

在script中引用：

```javascript
import HmCallOptionCard from '@/components/hm-call-option-card/index.vue'
export default {
    components: { HmCallOptionCard }
}
```

在template中使用：

```html
<template>
  <div class="test-component">
    <hm-call-option-card :options="options"></hm-call-option-card>
  </div>
</template>
<script>
import HmCallOptionCard from '@/components/hm-components/hm-call-option-card/index.vue'

export default {
  components: { HmCallOptionCard },
  data() {
    return {
      options: {
        yaoqingjiangli:
      '/static/hm-call-option-card/images/img_26361_0_0.png',
        title: '我们会给您回电话的',
        help: '帮助',
        date: '24/7',
        phoneIcon: 'phone',
        phone: '8 800 3254486',
        startChat: '发起聊天',
        voiceCall: '语音电话'
      }
    };
  },
  methods: {
    onClick: function(e) {
      console.log('onClick');
    }
  }
};
</script>
<style>
</style>
```

## 属性说明

| 属性名        | 类型     | 默认值 | 说明                                                                       |
|-----------   |---------|--------|----------------------------------------------------------------------------|
| options        | Object  | -      | 卡片属性                                                                   |

options对象各个属性说明如下：

| 属性名        | 类型     | 默认值 | 说明                                                                       |
|-----------   |---------|--------|----------------------------------------------------------------------------|
| title        | String  | -      | 标题文字                                                                   |
| help        | String  | -      | 帮助                                                                   |
| yaoqingjiangli        | String  | -      | 图片                                                                   |
| date        | String  | -      | 日期                                                                   |
| phoneIcon        | String  | -      | 电话                                                                   |
| phone        | String  | -      | 电话号码                                                                   |
| startChat        | String  | -      | 发起聊天按钮                                                                   |
| voiceCall        | String  | -      | 语音电话按钮                                                                   |

## 事件说明

| 事件称名   | 事件说明           | 返回参数 |
|----------|--------------------|----------|
| @click   | 点击 Card 触发事件 | -        |

## 更新日志

### 0.0.1(2020-04-02)

* 完成第一个版本