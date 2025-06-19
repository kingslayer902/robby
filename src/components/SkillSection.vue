<template>
  <section class="py-12 px-6 bg-white text-gray-800">
    <div class="max-w-3xl mx-auto">
      <h2 class="text-3xl font-bold mb-8 text-center">Kemampuan</h2>
      <div class="space-y-6">
        <SkillProgress label="Microsoft Word" percent="82" />
        <SkillProgress label="Microsoft Excel" percent="65" />
        <SkillProgress label="PowerPoint" percent="42" />
        <SkillProgress label="Presentasi" percent="90" />
        <SkillProgress label="Kerjasama Tim" percent="88" />
      </div>
    </div>
  </section>
</template>

<script setup>
import SkillProgress from './SkillProgress.vue'
</script>
