<template>
  <div id="basicLayout">
    <a-layout>
      <a-layout-header class="header">
        <GlobelHeader />
      </a-layout-header>
      <a-layout-content class="content">
        <router-view />
      </a-layout-content>

      <a-layout-footer class="footer">
        <a href="https://www.baidu.com" target="_blank">
          一站式用户管理中心 by May
        </a>
      </a-layout-footer></a-layout
    >
  </div>
</template>

<script setup lang="ts">
import GlobelHeader from '@/components/GlobelHeader.vue'
</script>

<style scoped>
#basicLayout .header {
  padding-inline: 20px;
  margin-bottom: 16px;
  color: unset;
  background: white;
}
#basicLayout .footer {
  background: #efefef;
  padding: 16px;
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  text-align: center;
}

#basicLayout .content {
  background: linear-gradient(to right, #fefefe, #fff);
  margin-bottom: 28px;
  padding: 20px;
}
</style>
