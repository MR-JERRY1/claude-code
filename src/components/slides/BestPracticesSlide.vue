<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
      <div class="max-w-6xl w-full">
        <h2 class="text-3xl font-bold mb-6 text-center gradient-text">Best Practices</h2>
        <p class="text-center opacity-80 mb-12 max-w-2xl mx-auto">Master the art of AI development - optimize performance, maximize ROI</p>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <ServerIcon class="w-5 h-5" />
              Extended Thinking Mode
            </h3>
            <p class="text-sm opacity-80 leading-relaxed">Use "think" < "think hard" < "think harder" < "ultrathink" for progressively more computation time. Significantly improves performance on complex problems.</p>
          </div>

          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <ComputerDesktopIcon class="w-5 h-5" />
              Context Window Optimization
            </h3>
            <p class="text-sm opacity-80 leading-relaxed">Use <code class="inline-code">/clear</code> regularly for stateless conversations. Different models offer varying context sizes - optimize usage based on task complexity. Configure forbidden directories in CLAUDE.md to prevent context pollution.</p>
          </div>

          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <ServerIcon class="w-5 h-5" />
              Model Selection Strategy
            </h3>
            <p class="text-sm opacity-80 leading-relaxed">Choose appropriate models for each task: more capable models for complex architectural decisions, efficient models for routine tasks. Subscription plans provide predictable costs vs pay-per-use pricing.</p>
          </div>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-8">
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <CheckCircleIcon class="w-5 h-5" />
              Automation Safeguards
            </h3>
            <p class="text-sm opacity-80 leading-relaxed">Set max_turns and timeout_minutes for CI/CD workflows. Use <code class="inline-code">/cost</code> command to monitor token usage patterns and prevent runaway costs.</p>
          </div>

          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <DocumentTextIcon class="w-5 h-5" />
              File Structure Strategy
            </h3>
            <p class="text-sm opacity-80 leading-relaxed">Create compact, single-purpose files. Use CLAUDE.md to specify reading boundaries and architectural patterns. Explicit file instructions prevent unnecessary token consumption.</p>
          </div>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-4">CLAUDE.md Configuration</h3>
            <div class="code-block rounded-lg p-4">
              <div class="text-xs opacity-60 mb-2">Project Configuration</div>
              <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># CLAUDE.md</span>
# Project: Vue TypeScript Dashboard

## Architecture
- Vue 3 with TypeScript
- Zustand for state management
- TanStack Query for data fetching
- Tailwind CSS for styling

## Forbidden Directories
- node_modules/
- .next/
- dist/
- coverage/

## Code Style
- Use functional components with hooks
- Prefer composition over inheritance
- Always include proper TypeScript types</pre>
            </div>
          </div>
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-4">Custom Command Workflow</h3>
            <div class="code-block rounded-lg p-4">
              <div class="text-xs opacity-60 mb-2">Automation Example</div>
              <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># .claude/commands/feature.md</span>
Implement $ARGUMENTS with the following requirements:

1. Create TypeScript interfaces for all data models
2. Use Vue Composition API for state management
3. Add comprehensive error handling
4. Include unit tests with 90%+ coverage
5. Update documentation and examples
6. Follow established naming conventions
7. Add accessibility attributes
8. Optimize for performance and bundle size

<span class="opacity-60"># Usage: claude /feature "user authentication flow"</span></pre>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ServerIcon, ComputerDesktopIcon, CheckCircleIcon, DocumentTextIcon } from '@heroicons/vue/24/outline'
</script>
