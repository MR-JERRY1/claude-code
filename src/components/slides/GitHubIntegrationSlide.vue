<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
      <div class="max-w-6xl w-full">
        <h2 class="text-3xl font-bold mb-6 text-center gradient-text">GitHub Integration</h2>
        <p class="text-center opacity-80 mb-12 max-w-2xl mx-auto">Context-aware intelligent PR reviews made simple</p>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <CodeBracketIcon class="w-5 h-5" />
              AI-Powered Security Reviews
            </h3>
            <p class="text-sm opacity-80 leading-relaxed">Automatically analyzes every PR for security vulnerabilities using deep semantic understanding. Diff-aware scanning focuses only on changed files.</p>
          </div>

          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <LinkIcon class="w-5 h-5" />
              @claude Mention Workflows
            </h3>
            <p class="text-sm opacity-80 leading-relaxed">Simple @claude mentions in PRs or issues trigger intelligent mode detection. Creates complete PRs, implements features, and fixes bugs while following project standards.</p>
          </div>

          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <AdjustmentsHorizontalIcon class="w-5 h-5" />
              Enterprise CI/CD Integration
            </h3>
            <p class="text-sm opacity-80 leading-relaxed">Integrates with existing pipelines, customizable security policies. Real-world impact: catches RCE vulnerabilities and DNS rebinding exploits before production.</p>
          </div>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-4">Setup GitHub Integration</h3>
            <div class="code-block rounded-lg p-4">
              <div class="text-xs opacity-60 mb-2">Installation</div>
              <pre class="text-sm opacity-80"><span class="opacity-60"># Install GitHub CLI</span>
brew install gh

<span class="opacity-60"># Authenticate and setup</span>
gh auth login
gh extension install anthropic/claude-code

<span class="opacity-60"># Install GitHub app</span>
claude /install-github-app</pre>
            </div>
          </div>

          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-4">@claude Mention Examples</h3>
            <div class="code-block rounded-lg p-4">
              <div class="text-xs opacity-60 mb-2">PR Comments</div>
              <pre class="text-sm opacity-80"><span class="opacity-60"># Security review</span>
@claude review this PR for security issues

<span class="opacity-60"># Feature implementation</span>
@claude implement dark mode toggle for Vue components

<span class="opacity-60"># Bug fix</span>
@claude fix the authentication bug in issue #42

<span class="opacity-60"># Code optimization</span>
@claude optimize the API response times</pre>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { CodeBracketIcon, LinkIcon, AdjustmentsHorizontalIcon } from '@heroicons/vue/24/outline'
</script>