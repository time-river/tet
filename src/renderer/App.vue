<template>
  <n-config-provider
    :locale="zhCN"
    :date-locale="dateZhCN"
    :theme="theme">
    <n-space vertical>

      <n-layout>
        <n-layout-header bordered>
          <n-card>
            <n-space>
              <n-button @click="theme = darkTheme">
                Dark
              </n-button>
              <n-button @click="theme = null">
                Light
              </n-button>
            </n-space>
          </n-card>
        </n-layout-header>
      </n-layout>

      <n-layout has-sider sider-placement="right">
        <n-layout-content content-style="padding: 24px;">
          Pingshan Road
        </n-layout-content>
        <n-layout-sider>
          Sidebar
        </n-layout-sider>
      </n-layout>
    </n-space>

  </n-config-provider>
</template>

<style scoped>
</style>

<script setup lang="js">
import { ref } from "vue";
import { darkTheme, zhCN, dateZhCN } from "naive-ui";

const theme = ref(null);
</script>
