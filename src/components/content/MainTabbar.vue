<template>
  <div id="mainTabbar">
    <tabbar>
      <tabbar-item path="/home">
        <template v-slot:defatullIcon>
          <img src="@/assets/img/tabbar/home.svg" />
        </template>
        <template v-slot:selectedIcon>
          <img src="@/assets/img/tabbar/home_active.svg" />
        </template>
        <template v-slot:itemText>
          <label>首页</label>
        </template>
      </tabbar-item>
      <tabbar-item path="/category">
        <template v-slot:defatullIcon>
          <img src="@/assets/img/tabbar/category.svg" />
        </template>
        <template v-slot:selectedIcon>
          <img src="@/assets/img/tabbar/category_active.svg" />
        </template>
        <template v-slot:itemText>
          <label>商品分类</label>
        </template>
      </tabbar-item>
      <tabbar-item path="/cart">
        <template v-slot:defatullIcon>
          <img src="@/assets/img/tabbar/shopcart.svg" />
        </template>
        <template v-slot:selectedIcon>
          <img src="@/assets/img/tabbar/shopcart_active.svg" />
        </template>
        <template v-slot:itemText>
          <label>购物车</label>
        </template>
      </tabbar-item>
      <tabbar-item path="/profile">
        <template v-slot:defatullIcon>
          <img src="@/assets/img/tabbar/profile.svg" />
        </template>
        <template v-slot:selectedIcon>
          <img src="@/assets/img/tabbar/profile_active.svg" />
        </template>
        <template v-slot:itemText>
          <label>我的</label>
        </template>
      </tabbar-item>
    </tabbar>
  </div>
</template>
<script>
import Tabbar from "@/components/common/tabbar/Tabbar.vue";
import TabbarItem from "@/components/common/tabbar/TabbarItem.vue";
export default {
  components: { TabbarItem, Tabbar },
  name: "MainTabbar",
};
</script>
<style scoped>
</style>
