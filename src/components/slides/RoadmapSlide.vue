<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
      <div class="max-w-6xl w-full">
        <h2 class="text-3xl font-bold mb-12 text-center gradient-text">Implementation Roadmap</h2>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-8">
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3">Phase 1: Pilot Projects</h3>
            <p class="text-sm opacity-80 leading-relaxed">Infrastructure assessment, security review, team training. Deploy on 2-3 pilot projects with disciplined Git workflows for safety isolation.</p>
          </div>

          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3">Phase 2: Team Standardization</h3>
            <p class="text-sm opacity-80 leading-relaxed">Codify standards in shared CLAUDE.md files. Create custom slash commands in <code class="inline-code">.claude/commands/</code> for team conventions and repetitive tasks.</p>
          </div>

          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3">Phase 3: Enterprise Integration</h3>
            <p class="text-sm opacity-80 leading-relaxed">Deploy GitHub App across all repositories. Integrate with existing CI/CD pipelines and security scanning tools. Scale subagent usage across development teams.</p>
          </div>

          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3">Phase 4: Advanced Automation</h3>
            <p class="text-sm opacity-80 leading-relaxed">Implement custom MCP servers for proprietary tools. Deploy autonomous bug fixing and feature development workflows. Full integration with business systems.</p>
          </div>
        </div>

      </div>
    </div>
  </div>
</template>

<script setup>
// No icons in this slide component
</script>
