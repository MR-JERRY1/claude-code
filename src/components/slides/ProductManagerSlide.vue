<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
    <div class="max-w-6xl w-full">
      <h2 class="text-3xl font-bold mb-6 text-center gradient-text">For Product Managers</h2>
      <p class="text-center opacity-80 mb-12 max-w-2xl mx-auto">Ship features 10x faster with AI-powered product development</p>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <DocumentTextIcon class="w-5 h-5" />
            PRD Generation
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Transform user interviews into comprehensive PRDs in minutes. Auto-generate acceptance criteria, success metrics, and technical requirements.</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <RocketLaunchIcon class="w-5 h-5" />
            Feature Validation
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Build working prototypes in hours, not weeks. Test with real users before committing engineering resources.</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <ChartBarIcon class="w-5 h-5" />
            Data-Driven Decisions
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Analyze user feedback, generate A/B test plans, and create automated dashboards for feature performance tracking.</p>
        </div>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">Real Scenario: Feature Launch</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">Monday → Friday Launch</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Monday: User Research</span>
Input: 50 customer interviews
Output: Synthesized insights, pain points ranked

<span class="opacity-60"># Tuesday: PRD Creation</span>
Generated: 15-page PRD with diagrams
Time saved: <span class="text-green-400">2 days → 30 minutes</span>

<span class="opacity-60"># Wednesday: Prototype</span>
Built: Interactive React prototype
User testing: 20 users, feedback analyzed

<span class="opacity-60"># Thursday: Refinement</span>
Updated: Specs based on feedback
Created: JIRA tickets, sprint planning

<span class="opacity-60"># Friday: Launch Ready</span>
Delivered: Complete feature package
Result: <span class="text-green-400">5x faster time-to-market</span></pre>
          </div>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">Custom Slash Commands</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">Example PM Commands You Can Create</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Generate user stories from PRD</span>
claude /stories "checkout flow PRD"
→ 25 user stories with acceptance criteria

<span class="opacity-60"># Competitive analysis</span>
claude /compete "payment solutions"
→ Feature matrix, pricing comparison

<span class="opacity-60"># Sprint planning</span>
claude /sprint "Q1 roadmap items"
→ Prioritized backlog, effort estimates

<span class="opacity-60"># Metrics dashboard</span>
claude /metrics "onboarding funnel"
→ SQL queries, Looker dashboard config

<span class="opacity-60"># Impact metrics</span>
Result: <span class="text-green-400">80% reduction in spec time</span>
Impact: <span class="text-green-400">3x more features shipped/quarter</span></pre>
          </div>
        </div>
      </div>
    </div>
    </div>
  </div>
</template>

<script setup>
import { DocumentTextIcon, RocketLaunchIcon, ChartBarIcon } from '@heroicons/vue/24/outline'
</script>