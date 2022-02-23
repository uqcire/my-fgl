<template>
  <n-config-provider :theme-overrides="themeOverrides">
    <main>
      <router-view></router-view>
    </main>
  </n-config-provider>
</template>

<script lang="ts" setup>
'App';

import { GlobalThemeOverrides, NConfigProvider } from 'naive-ui';
import theme from '@/styles/naive-ui-theme-overrides.json';

const themeOverrides: GlobalThemeOverrides = theme;
</script>
