<template>
  <div
    class="flex text-neutral-950 bg-neutral-50 dark:text-neutral-50 dark:bg-neutral-900"
  >
    <Header />
    <div
      class="flex flex-col gap-6 items-center justify-center w-100 h-134 m-2 px-8 py-8 rounded-md shrink-0 grow-0 bg-neutral-200 dark:bg-neutral-800"
    >
      <slot name="image" />
    </div>
    <div class="pr-16 pl-8 py-8">
      <h1 class="mt-4 text-2xl! font-bold">
        <slot name="title" />
      </h1>
      <div class="content-class mt-8 text-base leading-6">
        <slot name="content" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.content-class {
  @apply text-sm/6;
  :deep(h2) {
    @apply text-base font-bold mt-6 mb-2.5;
  }
  :deep(h3) {
    @apply text-sm font-bold mt-3 mb-1;
  }
  /* :deep(p) {
  } */
  :deep(li) {
    @apply my-1 leading-5.5 list-disc list-outside ml-[1.5em];
  }
}
</style>
