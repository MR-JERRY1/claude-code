<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
    <div class="max-w-6xl w-full">
      <h2 class="text-3xl font-bold mb-6 text-center gradient-text">For CTOs</h2>
      <p class="text-center opacity-80 mb-12 max-w-2xl mx-auto">Scale engineering productivity while maintaining architectural excellence</p>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <CpuChipIcon class="w-5 h-5" />
            Architecture Decisions
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Generate ADRs, evaluate tech stacks, and model system architectures. Predict scalability bottlenecks before they happen.</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <UserGroupIcon class="w-5 h-5" />
            Team Velocity
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">10x developer productivity with AI pair programming. Reduce onboarding from months to days with intelligent code understanding.</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <ShieldCheckIcon class="w-5 h-5" />
            Security & Quality
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Automated security scanning, code reviews, and technical debt analysis. Maintain SOC2 compliance with continuous monitoring.</p>
        </div>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">Transformation Impact</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">Before → After Claude Code</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Development Velocity</span>
Sprint velocity: 40 → <span class="text-green-400">120 story points</span>
Feature delivery: 2/month → <span class="text-green-400">8/month</span>
Bug rate: 15% → <span class="text-green-400">3%</span>

<span class="opacity-60"># Team Metrics</span>
Onboarding time: 3 months → <span class="text-green-400">1 week</span>
Code review time: 4 hours → <span class="text-green-400">30 minutes</span>
Documentation: 20% → <span class="text-green-400">100% coverage</span>

<span class="opacity-60"># Performance Impact</span>
Developer productivity: <span class="text-green-400">3x increase</span>
Infrastructure efficiency: <span class="text-green-400">40% improvement</span>
Time to market: <span class="text-green-400">75% faster</span>

<span class="opacity-60"># Engineering Metrics</span>
Team capacity: <span class="text-green-400">3x output increase</span>
Technical debt: <span class="text-green-400">60% reduction</span></pre>
          </div>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">Custom Slash Commands</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">Example CTO Commands You Can Create</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Architecture review</span>
claude /arch-review @microservices/
→ Bottleneck analysis, scaling recommendations

<span class="opacity-60"># Technical debt assessment</span>
claude /debt-scan --critical
→ Prioritized refactoring roadmap

<span class="opacity-60"># Security audit</span>
claude /security --compliance=SOC2
→ Vulnerability report, remediation plan

<span class="opacity-60"># Performance optimization</span>
claude /optimize --target=latency
→ Code improvements, 50% latency reduction

<span class="opacity-60"># Team analytics</span>
claude /team-metrics --quarter=Q4
→ Velocity trends, skill gap analysis

Results: <span class="text-green-400">Zero security incidents</span>
Scale: <span class="text-green-400">10M → 100M users handled</span></pre>
          </div>
        </div>
      </div>
    </div>
    </div>
  </div>
</template>

<script setup>
import { CpuChipIcon, UserGroupIcon, ShieldCheckIcon } from '@heroicons/vue/24/outline'
</script>