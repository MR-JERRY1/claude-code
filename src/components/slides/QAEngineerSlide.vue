<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
    <div class="max-w-6xl w-full">
      <h2 class="text-3xl font-bold mb-6 text-center gradient-text">For QA Engineers</h2>
      <p class="text-center opacity-80 mb-12 max-w-2xl mx-auto">Achieve 100% test coverage with intelligent automation</p>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <BeakerIcon class="w-5 h-5" />
            Test Generation
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Generate comprehensive test suites from requirements. Create unit, integration, E2E, and performance tests automatically.</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <BugAntIcon class="w-5 h-5" />
            Bug Detection
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">AI-powered bug prediction and root cause analysis. Reproduce complex bugs with generated test scenarios.</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <ArrowPathIcon class="w-5 h-5" />
            CI/CD Integration
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Automate regression testing, performance monitoring, and security scanning in your pipeline with zero manual intervention.</p>
        </div>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">Testing Transformation</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">E-Commerce Platform Testing</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Initial State</span>
Manual test cases: 500
Test execution: 2 weeks
Coverage: 45%

<span class="opacity-60"># With Claude Code</span>
Generated tests: <span class="text-green-400">5,000+ scenarios</span>
• Unit tests: 2,000 (Jest/Vitest)
• API tests: 1,500 (Postman/Newman)
• E2E tests: 1,000 (Playwright)
• Performance: 500 (K6/JMeter)

<span class="opacity-60"># Results After 1 Sprint</span>
Coverage: <span class="text-green-400">98.5%</span>
Execution time: <span class="text-green-400">45 minutes</span>
Bugs found: <span class="text-green-400">147 critical issues</span>
Prevention rate: <span class="text-green-400">95% defect reduction</span>

<span class="opacity-60"># Quality Impact</span>
QA time saved: <span class="text-green-400">90%</span>
Production bugs: <span class="text-green-400">85% reduction</span></pre>
          </div>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">Custom Slash Commands</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">Example QA Commands You Can Create</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Generate test suite</span>
claude /testgen @requirements.md
→ Complete test pyramid created

<span class="opacity-60"># Visual regression</span>
claude /visual-test --baseline
→ Pixel-perfect comparisons

<span class="opacity-60"># Load testing</span>
claude /perf --users=10000
→ K6 scripts, bottleneck analysis

<span class="opacity-60"># Security scanning</span>
claude /security-test --owasp
→ Penetration tests, CVE checks

<span class="opacity-60"># Accessibility audit</span>
claude /a11y --wcag=AA
→ Full compliance report

<span class="opacity-60"># Mobile testing</span>
claude /mobile-test --devices=all
→ Cross-device test matrix

Quality metrics: <span class="text-green-400">Zero escaped defects</span></pre>
          </div>
        </div>
      </div>
    </div>
    </div>
  </div>
</template>

<script setup>
import { BeakerIcon, BugAntIcon, ArrowPathIcon } from '@heroicons/vue/24/outline'
</script>