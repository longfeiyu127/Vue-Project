<template>
  <div id="app">
        <!-- 路由容器 -->
        <keep-alive>
            <router-view></router-view>
        </keep-alive>
        <!-- 切换按钮 -->
        <nav class="tabs">
            <router-link to="/index" class="tab">首页</router-link>
            <router-link to="/discover" class="tab">发现</router-link>
            <router-link to="/order" class="tab">订单</router-link>
            <router-link to="/profile" class="tab">我的</router-link>
        </nav>
    </div>
</template>

<script>
export default {
  name: "App"
};
</script>

<style lang="scss">
@import "./style/common.scss";
</style>
