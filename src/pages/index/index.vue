<template>
  <div>
    <i-grid i-class="no-border">
    <i-grid-item v-for="grid in grids" :key="grid" i-class="no-border">
        <i-grid-icon>
            <image :src="grid.image" />
        </i-grid-icon>
        <i-grid-label>{{grid.title}}</i-grid-label>
    </i-grid-item> 
    </i-grid>

      <i-panel :title="title_name">
          <view style="padding: 15px:">
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
        title_name:"热门",
        girds:[
            {title:"定语",image:"/static/images/user.png"},
            {title:"定语从句",image:"/static/images/user.png"},
            {title:"倒装句",image:"/static/images/user.png"},
            {title:"强调句",image:"/static/images/user.png"}
        ],
        top:[
            {name:"名字",address:"",image}
        ]
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
