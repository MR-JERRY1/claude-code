<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
      <div class="max-w-6xl w-full">
        <h2 class="text-3xl font-bold mb-6 text-center gradient-text">Custom Slash Commands</h2>
        <p class="text-center opacity-80 mb-12 max-w-2xl mx-auto">Standardize workflows with custom commands that capture your team's best practices</p>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <ArchiveBoxIcon class="w-5 h-5" />
              Dual Storage System
            </h3>
            <p class="text-sm opacity-80 leading-relaxed">Project commands in <code class="inline-code">.claude/commands/</code> (shared via git) and personal commands in <code class="inline-code">~/.claude/commands/</code></p>
          </div>
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <AdjustmentsHorizontalIcon class="w-5 h-5" />
              Dynamic Arguments
            </h3>
            <p class="text-sm opacity-80 leading-relaxed">Use <code class="inline-code">$ARGUMENTS</code> keyword for parameterized commands. Enables standardized workflows and consistent automation.</p>
          </div>
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <ComputerDesktopIcon class="w-5 h-5" />
              Professional Command Libraries
            </h3>
            <p class="text-sm opacity-80 leading-relaxed">Extensive libraries of pre-built commands available for code review, testing, security auditing, and business workflows. Community-driven with enterprise-grade quality.</p>
          </div>
        </div>

        <div class="card rounded-lg p-6 mb-8">
          <h3 class="text-xl font-semibold mb-4">Usage Examples</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">Command Usage</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Use built-in commands</span>
claude /code-review "authentication logic"
claude /fix-issue "#42"

<span class="opacity-60"># Create custom command</span>
echo "Implement $ARGUMENTS using Vue composition API and TypeScript" > .claude/commands/feature.md

<span class="opacity-60"># Use custom command</span>
claude /feature "user dashboard with real-time updates"</pre>
          </div>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-4">/code-review Command</h3>
            <div class="code-block rounded-lg p-4">
              <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Comprehensive Code Review</span>
Analyze recent changes for: $ARGUMENTS
1. Security vulnerabilities scan
2. Code quality assessment
3. Performance bottlenecks
4. Best practices compliance
5. Documentation completeness
6. Performance impact assessment</pre>
            </div>
          </div>
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-4">/fix-issue Command</h3>
            <div class="code-block rounded-lg p-4">
              <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># GitHub Issue Resolution</span>
Please analyze and fix GitHub issue: $ARGUMENTS
1. Understand the problem context
2. Identify root cause
3. Implement comprehensive solution
4. Add/update tests covering the fix
5. Update documentation if needed
6. Create conventional commit message</pre>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ArchiveBoxIcon, AdjustmentsHorizontalIcon, ComputerDesktopIcon } from '@heroicons/vue/24/outline'
</script>