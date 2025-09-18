<template>
  <div class="slide absolute inset-0 flex items-center justify-center text-center">
    <div class="max-w-5xl mx-auto px-8 animate-fade-in">
      <h1 class="text-6xl font-bold mb-8 gradient-text tracking-tight">Thank You!</h1>

      <div class="card rounded-xl p-8 max-w-4xl mx-auto text-center mb-8">
        <h2 class="text-lg font-semibold mb-6">Questions & Discussion</h2>
        <p class="opacity-80 leading-relaxed">
          Ready to explore how Claude Code can transform your development workflow?
        </p>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-6 max-w-4xl mx-auto">
        <div class="card rounded-lg p-4 text-center">
          <h3 class="font-semibold mb-2 flex items-center justify-center gap-2">
            <CodeBracketIcon class="w-5 h-5" />
            Implementation
          </h3>
          <p class="text-sm opacity-80">Setup strategies and best practices</p>
        </div>

        <div class="card rounded-lg p-4 text-center">
          <h3 class="font-semibold mb-2 flex items-center justify-center gap-2">
            <UsersIcon class="w-5 h-5" />
            Team Adoption
          </h3>
          <p class="text-sm opacity-80">Training and change management</p>
        </div>

        <div class="card rounded-lg p-4 text-center">
          <h3 class="font-semibold mb-2 flex items-center justify-center gap-2">
            <ShoppingBagIcon class="w-5 h-5" />
            Enterprise Integration
          </h3>
          <p class="text-sm opacity-80">Custom MCP servers and workflows</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { CodeBracketIcon, UsersIcon, ShoppingBagIcon } from '@heroicons/vue/24/outline'
</script>