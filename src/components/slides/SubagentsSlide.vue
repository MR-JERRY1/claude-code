<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
      <div class="max-w-6xl w-full">
        <h2 class="text-3xl font-bold mb-6 text-center gradient-text">AI Subagents: Specialized Workers</h2>
        <p class="text-center opacity-80 mb-12 max-w-2xl mx-auto">Parallel processing with domain experts - each subagent optimized for specific development tasks</p>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-8">
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <CpuChipIcon class="w-5 h-5" />
              Orchestrator-Worker Pattern
            </h3>
            <p class="text-sm opacity-80 leading-relaxed">Claude Code coordinates specialized subagents working in parallel. Each operates in isolated context windows for deep task focus while maintaining coordination through the main orchestrator.</p>
          </div>
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <ChartBarIcon class="w-5 h-5" />
              Performance Gains
            </h3>
            <p class="text-sm opacity-80 leading-relaxed">Subagent orchestration significantly outperforms single-agent systems on complex multi-step tasks. Automatic task delegation enables parallel processing and specialized expertise application.</p>
          </div>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-4 gap-4 mb-8">
          <div class="card rounded-lg p-4">
            <h4 class="font-semibold mb-2">Development & Architecture</h4>
            <p class="text-sm opacity-80">Vue components, TypeScript interfaces, architectural decisions, code reviews</p>
          </div>
          <div class="card rounded-lg p-4">
            <h4 class="font-semibold mb-2">Language Specialists</h4>
            <p class="text-sm opacity-80">Framework-specific experts: Vue/Nuxt.js, Node.js/Express, Python/FastAPI specialists</p>
          </div>
          <div class="card rounded-lg p-4">
            <h4 class="font-semibold mb-2">Quality Assurance</h4>
            <p class="text-sm opacity-80">Vitest testing, security auditing, code quality, accessibility compliance</p>
          </div>
          <div class="card rounded-lg p-4">
            <h4 class="font-semibold mb-2">Infrastructure & Operations</h4>
            <p class="text-sm opacity-80">CI/CD pipelines, Docker configs, cloud deployment (Azure), monitoring setup</p>
          </div>
        </div>

        <div class="card rounded-lg p-6 mb-6">
          <h3 class="text-xl font-semibold mb-4">Subagent Usage Example</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">Parallel Task Execution</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Deploy multiple specialists simultaneously</span>
claude "Build a Vue dashboard with real-time analytics"

<span class="opacity-60"># Orchestrator automatically delegates:</span>
┌─ Frontend Agent: Vue components + TypeScript
├─ Backend Agent: API endpoints + database models
├─ Testing Agent: Unit tests + integration tests
└─ DevOps Agent: Docker + deployment config</pre>
          </div>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <UsersIcon class="w-5 h-5" />
            Community Ecosystem
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Growing library of production-ready subagents available from the community. Project-specific agents in <code class="inline-code">.claude/commands/</code> override global ones. Easy sharing through portable configuration files.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { CpuChipIcon, ChartBarIcon, UsersIcon } from '@heroicons/vue/24/outline'
</script>