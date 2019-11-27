<template>
  <div>
    <swiper
      :indicator-dots="indicatorDots"
      :autoplay="autoplay"
      :interval="interval"
      :duration="duration"
      
    >
      <block v-for="img in imgUrls" :key="img">
        <swiper-item>
          <image :src="img" style="width:100%" />
        </swiper-item>
      </block>
    </swiper>
    <i-grid i-class="no-border">
    <i-grid-item @click="goType(grid)" v-for="grid in grids" :key="grid" i-class="no-border">
        <i-grid-icon>
            <image :src="grid.image" />
        </i-grid-icon>
        <i-grid-label>{{grid.title}}</i-grid-label>
    </i-grid-item>
  </i-grid>

   <i-grid i-class="no-border">
    <i-grid-item @click="goType(krid)" v-for="krid in krids" :key="krid" i-class="no-border">
        <i-grid-icon>
            <image :src="krid.image" />
        </i-grid-icon>
        <i-grid-label>{{krid.title}}</i-grid-label>
    </i-grid-item>
  </i-grid>

  </div>
</template>

<script>
export default {
  data () {
    return {

      grids: [
        {title:"定语",image:"/static/images/1.png"},
        {title:"定语从句",image:"/static/images/2.png"},
        {title:"倒装句",image:"/static/images/3.png"},
        {title:"强调句",image:"/static/images/4.png"}
      ],

      krids: [
        {title:"状语",image:"/static/images/5.png"},
        {title:"主语从句",image:"/static/images/6.png"},
        {title:"动词",image:"/static/images/7.png"},
        {title:"宾语从句",image:"/static/images/8.png"}
      ],

   
      imgUrls: [
        'https://images.unsplash.com/photo-1551334787-21e6bd3ab135?w=640',
        'https://images.unsplash.com/photo-1551214012-84f95e060dee?w=640',
        'https://images.unsplash.com/photo-1551446591-142875a901a1?w=640'
      ],
      indicatorDots: false,
      autoplay: false,
      interval: 5000,
      duration: 1000
    }
  },

  methods: {
    goType(type){
      console.log(type)
      let url = '../list/main?type=' + type.title
      mpvue.navigateTo({ url })
    }
  },

  created () {
    const db = wx.cloud.database({ env: 'edu-868a10' })
    db.collection('top').get().then(
      res => {
        console.log(res.data)
        this.top = res.data
  }
  )
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
