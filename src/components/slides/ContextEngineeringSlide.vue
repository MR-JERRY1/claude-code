<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
    <div class="max-w-6xl w-full">
      <h2 class="text-3xl font-bold mb-6 text-center gradient-text">Context Engineering</h2>
      <p class="text-center opacity-80 mb-12 max-w-2xl mx-auto">Lessons from production: Why context quality beats agent quantity</p>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <XMarkIcon class="w-5 h-5" />
            Multi-Agent Pitfalls
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Agents misinterpret tasks, produce inconsistent results. Example: Flappy Bird clone with Mario background, mismatched assets.</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <CheckCircleIcon class="w-5 h-5" />
            Linear Architecture
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Single-threaded processing with full context. One agent sees entire history, decisions remain consistent.</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <ServerIcon class="w-5 h-5" />
            Context Compression
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Specialized LLM summarizes action history. Manages 100K+ tokens while preserving key decisions.</p>
        </div>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">Production Wins</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">Real-World Impact</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Cisco Outshift - CI/CD Setup</span>
Before: 1 week manual setup
After:  1 hour automated → <span class="text-green-400">10x faster</span>

<span class="opacity-60"># Captide - Investment Research</span>
Before: Days of analysis
After:  Seconds to complete → <span class="text-green-400">1000x faster</span>

<span class="opacity-60"># Webtoon - Story Understanding</span>
Scale: Marketing, translation, recommendations
Impact: Enterprise-wide deployment</pre>
          </div>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">Context Pattern</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">Implementation Guide</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># AVOID: Parallel multi-agent</span>
Task → Agent1 ─┐
     → Agent2 ─┼→ Merge → Conflicts
     → Agent3 ─┘

<span class="opacity-60"># USE: Linear with compression</span>
Full Context → Compression → Single Agent

<span class="opacity-60"># Key Principles:</span>
1. Share complete agent traces
2. Compress every N actions
3. Preserve architectural decisions
4. Maintain continuous context</pre>
          </div>
        </div>
      </div>
    </div>
    </div>
  </div>
</template>

<script setup>
import { XMarkIcon, CheckCircleIcon, ServerIcon } from '@heroicons/vue/24/outline'
</script>

<style scoped>
.bg-size-200 {
  background-size: 200% 200%;
}

@keyframes gradient {
  0%, 100% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
}

.animate-gradient {
  animation: gradient 3s ease infinite;
}
</style>