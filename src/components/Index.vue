<template>
    <div class="page" id="index">
        <h1>Index</h1>
        <ul class="list">
            <li class="item" v-for="(item,index) in dataList" :key="index">
                <router-link to="/index/detail?5=2">{{item}}</router-link>
            </li>
        </ul>
        <transition enter-active-class="slideInRight animation-timing-300"
                    leave-active-class="slideOutRight animation-timing-300">
            <router-view></router-view>
        </transition>
    </div>
</template>

<script>
export default {
  data() {
    return {
      dataList: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
    };
  }
};
</script>

<style lang="scss">
@import "../style/index.scss";
</style>
