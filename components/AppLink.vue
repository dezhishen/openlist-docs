<script setup lang="ts">
  // https://router.vuejs.org/guide/advanced/extending-router-link.html#extending-routerlink
  import { computed } from 'vue'
  const props = defineProps<{
    showExternalIcon?: boolean
    external?: boolean
    to?: string
    href?: string
  }>()
  const link = computed(() => props.href || props.to || '#')
  const isExternalLink = computed(() => {
    return typeof link.value === 'string' && link.value.startsWith('http')
  })
</script>

<template>
  <a v-if="isExternalLink" v-bind="$attrs" :href="link" target="_blank">
    <slot />
    <div v-if="showExternalIcon" class="icon-link inline-block" i-ri-arrow-right-up-line />
  </a>
  <RouterLink
    v-else-if="!isExternalLink && props.external"
    v-bind="$attrs"
    :to="link"
    tag="a"
    target="_blank"
  >
    <slot />
    <div v-if="showExternalIcon" class="icon-link inline-block" i-ri-arrow-right-up-line />
  </RouterLink>
  <RouterLink v-else v-bind="$attrs" :to="link">
    <slot />
  </RouterLink>
</template>
