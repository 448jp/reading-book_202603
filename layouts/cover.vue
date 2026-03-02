<script setup lang="ts">
import TitleRenderer from "#slidev/title-renderer";
</script>

<template>
  <div
    class="flex text-neutral-950 bg-neutral-50 dark:text-neutral-50 dark:bg-neutral-900"
  >
    <div class="flex items-center justify-center w-100 h-138 shrink-0 grow-0">
      <slot name="cover" />
    </div>
    <div class="p-16">
      <div class="flex items-center gap-2 text-sm">
        <div
          class="bg-neutral-200 w-fit px-2.5 py-1 rounded-sm font-bold dark:bg-neutral-800"
        >
          <slot name="date" />
        </div>
        <div class="font-bold">読書感想会</div>
      </div>
      <h1 class="mt-4 text-2xl! font-bold">
        <TitleRenderer />
      </h1>
      <div class="mt-4 text-xs/4.5">
        <slot name="description" />
      </div>
      <div class="mt-8 flex items-center gap-2">
        <div aria-hidden="true" class="w-1 h-4 bg-neutral-400"></div>
        <h2 class="text-base! font-bold">概要</h2>
      </div>
      <p class="text-sm! mt-2! leading-[1.6]!">
        <slot name="overview" />
      </p>
    </div>
  </div>
</template>
