<template>
  <div
    class="h-138 p-16 text-neutral-950 bg-neutral-50 dark:text-neutral-50 dark:bg-neutral-900"
  >
    <Header />
    <div class="w-full">
      <h1 class="text-3xl! font-bold font-serif">
        <slot name="title" />
      </h1>
      <div class="content-class mt-10 text-base leading-6">
        <slot name="content" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.content-class {
  @apply text-sm/6;
  :deep(h2) {
    @apply text-lg font-bold mt-8 mb-2.5;
  }
  :deep(h3) {
    @apply text-sm font-bold mt-4 mb-1;
  }
  /* :deep(p) {
  } */
  :deep(li) {
    @apply my-1 leading-5.5 list-disc list-outside ml-[1.5em];
  }
}
</style>
