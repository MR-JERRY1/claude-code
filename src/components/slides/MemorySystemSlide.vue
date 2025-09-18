<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
    <div class="max-w-6xl w-full">
      <h2 class="text-3xl font-bold mb-6 text-center gradient-text">Smart Memory System</h2>
      <p class="text-center opacity-80 mb-12 max-w-2xl mx-auto">Context that follows you through every project phase</p>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <FolderIcon class="w-5 h-5" />
            Hierarchical Memory
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Claude Code reads memories recursively from current directory up
            to project root. Use <code class="inline-code">/init</code> command to create shared context.</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <LinkIcon class="w-5 h-5" />
            Dynamic Imports
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Use <code class="inline-code">@path/to/file</code>
            syntax to import additional context. Files load automatically at session start.</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <CheckCircleIcon class="w-5 h-5" />
            Best Practices
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Include architecture decisions, coding conventions, API
            patterns. Keep lean - use <code class="inline-code">/memory</code> to manage context.</p>
        </div>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">CLAUDE.md Example</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">Project Memory File</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Project Context</span>

<span class="text-sm opacity-80">## Architecture</span>
- Vue frontend with TypeScript
- Node.js backend with Express
- MongoDB database with Mongoose ODM

<span class="text-sm opacity-80">## Conventions</span>
- Use PascalCase for component files
- All API routes start with /api/v1/
- Test files end with .test.ts

<span class="text-sm opacity-80">## Dependencies</span>
@components/ui/Button.tsx
@utils/validation.ts</pre>
          </div>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">Dynamic Imports</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">Usage Examples</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Import specific files</span>
claude "Fix the login bug" @src/auth/login.ts

<span class="opacity-60"># Import directory context</span>
claude "Add tests" @tests/

<span class="opacity-60"># Multiple file context</span>
claude "Refactor API" @api/users.ts @api/auth.ts

<span class="opacity-60"># Auto-loaded in CLAUDE.md</span>
@shared/types.ts
@config/database.ts</pre>
          </div>
        </div>
      </div>
    </div>
    </div>
  </div>
</template>

<script setup>
import { FolderIcon, LinkIcon, CheckCircleIcon } from '@heroicons/vue/24/outline'
</script>