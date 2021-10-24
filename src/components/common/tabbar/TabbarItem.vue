<template>
  <div class="tabbar-item" @click="itemClick">
    <div class="selectedIcon" v-if="isActive"><slot name="selectedIcon"></slot></div>
    <div class="defaultIcon" v-else><slot name="defatullIcon"></slot></div>
    <div :style="activeStype" class="title"><slot name="itemText"></slot></div>
  </div>
</template>
<script>
export default {
  name: "TabbarItem",
  props: {
    path:String,
    active_color:{
      type:String,
      default:'red'
    }
  },
  computed: {
    isActive() {
      return (this.$route.path.indexOf(this.path)) !== -1;
    },
    activeStype(){
      return this.isActive ? {color:this.active_color}:{}
    }
  },
  methods:{
    itemClick(){
      this.$router.replace(this.path)
    }
  }
};
</script>
<style>
  .tabbar-item{
    flex:1;
    text-align: center;
  }
  .defaultIcon img,.selectedIcon img{
    width: 24px;
    height: 24px;
  }
  .title{
    font-size: 12px;
  }

</style>
