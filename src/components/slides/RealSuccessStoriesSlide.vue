<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
    <div class="max-w-6xl w-full">
      <h2 class="text-3xl font-bold mb-6 text-center gradient-text">Real Success Stories</h2>
      <p class="text-center opacity-80 mb-8 max-w-2xl mx-auto">Companies achieving breakthrough results with Claude Code in production</p>
      <div class="text-center mb-8">
        <a href="https://claude.com/customers/rakuten" target="_blank" class="text-cyan-400 hover:text-cyan-300 text-sm mx-2">Rakuten Case Study</a>
        <span class="opacity-40">|</span>
        <a href="https://www.anthropic.com/news/claude-code-on-team-and-enterprise" target="_blank" class="text-cyan-400 hover:text-cyan-300 text-sm mx-2">Behavox Story</a>
        <span class="opacity-40">|</span>
        <a href="https://news.ycombinator.com/item?id=45163362" target="_blank" class="text-cyan-400 hover:text-cyan-300 text-sm mx-2">Kernel Driver Project</a>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <BuildingOfficeIcon class="w-5 h-5" />
            Rakuten
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Japanese tech giant's ML engineer completed 12.5M lines of code implementation in <strong>7 hours autonomous work</strong>. 99.9% accuracy achieved.</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <ShieldCheckIcon class="w-5 h-5" />
            Behavox
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Compliance company deployed to <strong>hundreds of developers</strong>. "Consistently outperforms other agents, delivering superior results daily."</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <GlobeAltIcon class="w-5 h-5" />
            Altana
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">AI-powered supply chain network experiencing <strong>transformational results</strong> across global operations with Claude Code integration.</p>
        </div>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">Rakuten Case Study</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">vLLM Implementation Challenge</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># The Challenge</span>
Task: Implement activation vector extraction
Codebase: 12.5 million lines of code
Languages: Multiple programming languages

<span class="opacity-60"># The Result</span>
Time: <span class="text-green-400">7 hours fully autonomous</span>
Human code: <span class="text-green-400">Zero lines written</span>
Accuracy: <span class="text-green-400">99.9% numerical accuracy</span>

<span class="opacity-60"># Impact</span>
• Non-engineers now contribute to coding
• Terminal interface as safety guardrail
• Accelerated time to market

"I didn't write any code during those
seven hours" - Kenta Naruse, ML Engineer

<a href="https://claude.com/customers/rakuten" target="_blank" class="text-cyan-400 hover:text-cyan-300 text-xs">→ Read full case study</a></pre>
          </div>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">Individual Success Stories</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">From Zero to Revenue</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># William Roberts - Founder</span>
Starting point: Zero coding knowledge
Time to MVP: <span class="text-green-400">3 days</span>
Revenue milestone: <span class="text-green-400">First $1,000 in 4 months</span>

<span class="opacity-60"># 25-Year Kernel Driver</span>
Legacy code: Successfully modernized
Result: <span class="text-green-400">10x faster implementation</span>

<span class="opacity-60"># Developer Testimonials</span>
"Haven't typed a function in weeks,
yet shipping faster than ever"

"Saved 6-10 hours on single project"

"Made me cancel Cursor, Copilot & ChatGPT"

<span class="text-xs opacity-60">Sources:</span>
<a href="https://www.arsturn.com/blog/from-zero-to-deployed-how-founder-built-app-with-claude-code" target="_blank" class="text-cyan-400 hover:text-cyan-300 text-xs">→ Founder Story</a>
<a href="https://medium.com/@george.vetticaden/claude-code-the-agentic-development-revolution-that-made-me-cancel-cursor-copilot-chatgpt-67508130e2e5" target="_blank" class="text-cyan-400 hover:text-cyan-300 text-xs">→ Cancel Everything</a>
<a href="https://every.to/source-code/how-i-use-claude-code-to-ship-like-a-team-of-five" target="_blank" class="text-cyan-400 hover:text-cyan-300 text-xs">→ Ship Like Team of 5</a></pre>
          </div>
        </div>
      </div>
    </div>
    </div>
  </div>
</template>

<script setup>
import { BuildingOfficeIcon, ShieldCheckIcon, GlobeAltIcon } from '@heroicons/vue/24/outline'
</script>