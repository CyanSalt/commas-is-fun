<script lang="ts" setup>
import FunPane from './components/FunPane.vue'
</script>

<template>
  <FunPane />
</template>

<style lang="scss" scoped>
:global(:root) {
  --design-green: 40 201 65;
  --design-yellow: 255 189 46;
  --design-red: 255 97 89;
  --design-blue: 47 136 255;
  --design-magenta: 207 150 253;
  --design-cyan: 0 200 210;
  --theme-foreground: 192 197 206;
  --theme-background: 27 43 52;
  --theme-selection: 110 120 129;
  --theme-black: 27 43 52;
  --theme-red: 236 95 103;
  --theme-green: 153 199 148;
  --theme-yellow: 250 200 99;
  --theme-blue: 102 153 204;
  --theme-magenta: 197 148 197;
  --theme-cyan: 95 179 179;
  --theme-white: 255 255 255;
}
:global(body) {
  margin: 0;
  color: rgb(var(--theme-foreground));
  font-family: Fira Code, Cascadia Code, Consolas, Monaco, Andale Mono, Ubuntu Mono, monospace;
  font-size: 14px;
  background: rgb(var(--theme-background));
}
.fun-pane {
  max-width: 640px;
  margin: auto;
}
:deep(.form-line-tip) {
  flex-basis: 100%;
  margin-bottom: 8px;
  font-style: italic;
  font-size: 12px;
  line-height: 24px;
  &::before {
    content: '*';
    margin-right: 1em;
  }
}
</style>
