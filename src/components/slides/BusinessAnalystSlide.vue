<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
    <div class="max-w-6xl w-full">
      <h2 class="text-3xl font-bold mb-6 text-center gradient-text">For Business Analysts</h2>
      <p class="text-center opacity-80 mb-12 max-w-2xl mx-auto">Transform complex requirements into clear solutions at enterprise scale</p>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <DocumentDuplicateIcon class="w-5 h-5" />
            Requirements Automation
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Convert stakeholder meetings into BRDs, FRDs, and technical specs. Auto-generate traceability matrices and gap analyses.</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <CubeTransparentIcon class="w-5 h-5" />
            Process Modeling
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Create BPMN diagrams, data flow charts, and system architecture from requirements. Identify bottlenecks automatically.</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <PresentationChartLineIcon class="w-5 h-5" />
            Impact Analysis
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Assess change impacts across systems. Generate test scenarios, risk matrices, and mitigation strategies instantly.</p>
        </div>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">Case Study: ERP Migration</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">6-Month Project → 3 Weeks</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Week 1: Discovery</span>
Analyzed: 500+ business processes
Interviewed: 50 stakeholders
Generated: Complete AS-IS documentation

<span class="opacity-60"># Week 2: Gap Analysis</span>
Identified: 127 gaps, 45 critical
Created: Risk mitigation plans
Output: <span class="text-green-400">200-page analysis in 2 days</span>

<span class="opacity-60"># Week 3: Solution Design</span>
Designed: TO-BE processes
Generated: 1,500 test cases
Created: Data migration mappings

<span class="opacity-60"># Results</span>
Time saved: <span class="text-green-400">85% reduction</span>
Accuracy: <span class="text-green-400">99.2% requirement coverage</span>
Defects: <span class="text-green-400">Zero requirements defects</span></pre>
          </div>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">Custom Slash Commands</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">Example BA Commands You Can Create</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Requirements extraction</span>
claude /extract @meeting-notes.txt
→ BRD, FRD, Use Cases, User Stories

<span class="opacity-60"># Data model generation</span>
claude /datamodel "inventory system"
→ ERD, Data dictionary, SQL schemas

<span class="opacity-60"># Process optimization</span>
claude /optimize @current-process.bpmn
→ Bottleneck analysis, recommendations

<span class="opacity-60"># Test scenario creation</span>
claude /testgen @requirements.doc
→ 500+ test cases with edge cases

<span class="opacity-60"># Stakeholder reports</span>
Automated: <span class="text-green-400">Daily progress dashboards</span>
Quality: <span class="text-green-400">Zero defects in requirements</span></pre>
          </div>
        </div>
      </div>
    </div>
    </div>
  </div>
</template>

<script setup>
import { DocumentDuplicateIcon, CubeTransparentIcon, PresentationChartLineIcon } from '@heroicons/vue/24/outline'
</script>