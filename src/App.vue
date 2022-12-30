<template>
  <div class="bg-base h-real w-full">
    <div
      class="max-w-md mx-auto h-full w-full flex flex-col justify-between p-5 px-10"
    >
      <div class="grow flex flex-col items-center">
        <div class="flex gap-1 items-center mb-10">
          <img src="./assets/Logo.png" class="h-10" />
          <h2 class="text-2xl">OpenNCCU Beta</h2>
        </div>
        <a
          class="shadow-numo w-full rounded-xl p-4 flex gap-3 items-center"
          href="/scsr"
        >
          <img src="./assets/GDSCSCSR.png" class="h-8" />
          <h2 class="text-xl font-bold">OpenNCCU 選課系統</h2>
        </a>
      </div>
      <div class="shrink-0 text-center">2022 - 2022 @ OpenNCCU</div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { onMounted } from "vue";

onMounted(() => {
  const documentHeight = () => {
    const doc = document.documentElement;
    doc.style.setProperty("--doc-height", `${window.innerHeight}px`);
  };
  window.addEventListener("resize", documentHeight);
  documentHeight();
});
</script>
