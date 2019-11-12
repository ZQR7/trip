<template>
  <div>
    <i-grid i-class="no-border">
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="/static/images/user.png" />
        </i-grid-icon>
        <i-grid-label>定语</i-grid-label>
    </i-grid-item>
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="/static/images/user.png" />
        </i-grid-icon>
        <i-grid-label>Grid</i-grid-label>
    </i-grid-item >
        <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="/static/images/user.png" />
        </i-grid-icon>
        <i-grid-label>Grid</i-grid-label>
    </i-grid-item>
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="/static/images/user.png" />
        </i-grid-icon>
        <i-grid-label>Grid</i-grid-label>
    </i-grid-item>
  </i-grid>
  <i-panel title="热门">
    <view style="padding: 15px;">
      <i-card i-class="split" title="卡片标题" extra="额外内容" thumb="https://i.loli.net/2017/08/21/599a521472424.jpg">
          <view slot="content">内容不错</view>
          <view slot="footer">尾部内容</view>
      </i-card>
      <i-card i-class="split" title="卡片标题" extra="额外内容" thumb="https://i.loli.net/2017/08/21/599a521472424.jpg">
          <view slot="content">内容不错</view>
          <view slot="footer">尾部内容</view>
      </i-card>
      <i-card i-class="split" title="卡片标题" extra="额外内容" thumb="https://i.loli.net/2017/08/21/599a521472424.jpg">
          <view slot="content">内容不错</view>
          <view slot="footer">尾部内容</view>
      </i-card>
    </view>
  </i-panel>
  </div>
</template>

<script>
export default {
  data () {
    return {
    }
  },

  methods: { 
   },

  created () {
 }
}
</script>

<style scoped>
div >>> .no-border {
  border-width: 0pt;
}
div >>> .split {
  margin-bottom: 10pt;
}
</style>
