<template>
  <view>
    <view>
      <view class="cu-custom" style="height: 50px">
        <view
          class="cu-bar fixed sbyw-bg-blue"
          style="height: 50px; padding-top: 0px"
        >
          <view class="action">
            <text class="iconfont icon-cui-icon_fanhui"></text>
          </view>
          <view class="content" style="top: 0px"> 社保缴费证明查验</view>
          <view class="action"></view>
        </view>
        <view></view>
      </view>
    </view>
    <view
      style="
        position: fixed;
        z-index: 10;
        color: red;
        padding: 9px;
        font-size: 12px;
        background-color: rgb(255, 255, 255);
      "
    >
      长按图片可保存，如有多张图片，请长按每张图片进行保存。
    </view>
  </view>
</template>

<script>
export default {
  data() {
    return {
      title: "Hello",
    };
  },
  onLoad() {},
  methods: {},
};
</script>

<style>

.cu-custom {
  display: block;
  position: relative;
}
.cu-custom .cu-bar {
  min-height: 0;
  box-shadow: 0px 0px 0px;
  z-index: 999;
}
.cu-bar.fixed,
.nav.fixed {
  position: fixed;
  width: 100%;
  top: 0;
  z-index: 1024;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.1);
}
.cu-bar {
  display: flex;
  position: relative;
  align-items: center;
  min-height: 48px;
  justify-content: space-between;
}
.sbyw-bg-blue {
  background-color: #168de9;
  color: #fff;
}
.cu-bar .action:first-child {
  margin-left: 14px;
  font-size: 14px;
}
.cu-bar .action {
  display: flex;
  align-items: center;
  height: 100%;
  justify-content: center;
  max-width: 100%;
}
.cu-bar .content {
  position: absolute;
  text-align: center;
  width: calc(100% - 163px);
  left: 0;
  right: 0;
  bottom: 0;
  top: 0;
  margin: auto;
  height: 28px;
  font-size: 15px;
  line-height: 28px;
  cursor: none;
  pointer-events: none;
  text-overflow: ellipsis;
  white-space: nowrap;
  overflow: hidden;
}
.cu-bar .action:last-child {
  margin-right: 14px;
}

.cu-bar .action {
  display: flex;
  align-items: center;
  height: 100%;
  justify-content: center;
  max-width: 100%;
}
</style>
