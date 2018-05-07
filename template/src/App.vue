<script>
export default {
  created () {
    // 调用API从本地缓存中获取数据
    // eslint-disable-next-line
    const logs = wx.getStorageSync('logs') || []
    logs.unshift(Date.now())
    // eslint-disable-next-line
    wx.setStorageSync('logs', logs)

    console.log('app created and cache logs by setStorageSync')
  }
}
</script>

<style>
.container {
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  padding: 200rpx 0;
  box-sizing: border-box;
}
</style>
