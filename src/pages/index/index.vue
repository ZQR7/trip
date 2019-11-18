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
        <i-grid-label>定语从句</i-grid-label>
    </i-grid-item >
        <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="/static/images/user.png" />
        </i-grid-icon>
        <i-grid-label>倒装句</i-grid-label>
    </i-grid-item>
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="/static/images/user.png" />
        </i-grid-icon>
        <i-grid-label>强调句</i-grid-label>
    </i-grid-item>
   
  </i-grid>
    <i-grid i-class="no-border">
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="/static/images/user.png" />
        </i-grid-icon>
        <i-grid-label>状语</i-grid-label>
    </i-grid-item>
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="/static/images/user.png" />
        </i-grid-icon>
        <i-grid-label>动词</i-grid-label>
    </i-grid-item >
        <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="/static/images/user.png" />
        </i-grid-icon>
        <i-grid-label>状语从句</i-grid-label>
    </i-grid-item>
    <i-grid-item i-class="no-border">
        <i-grid-icon>
            <image src="/static/images/user.png" />
        </i-grid-icon>
        <i-grid-label>宾语从句</i-grid-label>
    </i-grid-item>
  
  </i-grid>
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
