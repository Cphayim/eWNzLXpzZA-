<style type="less">

</style>
<template>
  <view>
    <view>爸爸说：{{num}}</view>
    <view @tap="childTap">{{msg}}</view>
    <slot></slot>
  </view>
</template>

<script>
import Wepy from 'wepy'

export default class Com1 extends Wepy.component {
  props = {
    num: Number
  }
  data = {
    msg: '我是Com1'
  }
  methods = {
    childTap() {
    }
  }
}
</script>
