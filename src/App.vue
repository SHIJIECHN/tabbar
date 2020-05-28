<template>
  <div id="app">
    <tab-bar>
        <tab-bar-item path="/home" activeColor="blue">
          <div slot="item-icon"><img src="./assets/img/home.png" alt=""></div>
          <div slot="item-icon-active"><img src="./assets/img/home-active.png" alt=""></div>
          <div slot="item-name">首页</div>
        </tab-bar-item>
        <tab-bar-item path="/category" activeColor="blue">
          <div slot="item-icon"><img src="./assets/img/category.png" alt=""></div>
          <div slot="item-icon-active"><img src="./assets/img/category-active.png" alt=""></div>
          <div slot="item-name">分类</div>
        </tab-bar-item>
        <tab-bar-item path="/cart" activeColor="blue">
          <div slot="item-icon"><img src="./assets/img/cart.png" alt=""></div>
          <div slot="item-icon-active"><img src="./assets/img/cart-active.png" alt=""></div>
          <div slot="item-name">购物车</div>
        </tab-bar-item>
        <tab-bar-item path="profile" activeColor="blue">
          <div slot="item-icon"><img src="./assets/img/profile.png" alt=""></div>
          <div slot="item-icon-active"><img src="./assets/img/profile-active.png" alt=""></div>
          <div slot="item-name">我的</div>
        </tab-bar-item>
    </tab-bar>
    <router-view/>
  </div>
</template>

<script>
  import TabBar from './components/tabbar/TabBar'
  import TabBarItem from "./components/tabbar/TabBarItem";

export default {
  name: 'App',
  components:{
    TabBar,
    TabBarItem
  }
}
</script>

<style>
 @import "./assets/style/common.css";
</style>
