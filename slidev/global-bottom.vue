<template>
  <footer
    v-if="$nav.currentLayout !== 'intro'"
    class="absolute bottom-2 right-2 text-xs opacity-50"
  >
    {{ $nav.currentPage }} / {{ $nav.total }}
  </footer>
</template> 