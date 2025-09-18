<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
      <div class="max-w-6xl w-full">
        <h2 class="text-3xl font-bold mb-6 text-center gradient-text">Tools & Model Context Protocol (MCP)</h2>
        <p class="text-center opacity-80 mb-12 max-w-2xl mx-auto">Connect to any system, automate any workflow, scale beyond limits</p>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-8">
          <div>
            <h3 class="text-lg font-semibold mb-4 flex items-center gap-2">
              <WrenchScrewdriverIcon class="w-5 h-5" />
              Built-in Tools
            </h3>
            <div class="space-y-3">
              <div class="card rounded-lg p-4">
                <strong class="block mb-1">File Operations</strong>
                <span class="text-sm opacity-80">Read, write, search across codebases</span>
              </div>
              <div class="card rounded-lg p-4">
                <strong class="block mb-1">Terminal Commands</strong>
                <span class="text-sm opacity-80">Run tests, builds, deployments</span>
              </div>
              <div class="card rounded-lg p-4">
                <strong class="block mb-1">Git Operations</strong>
                <span class="text-sm opacity-80">Branch, commit, merge, rebase</span>
              </div>
              <div class="card rounded-lg p-4">
                <strong class="block mb-1">Web Search</strong>
                <span class="text-sm opacity-80">Find current documentation and solutions</span>
              </div>
            </div>
          </div>

          <div>
            <h3 class="text-lg font-semibold mb-4 flex items-center gap-2">
              <CubeTransparentIcon class="w-5 h-5" />
              MCP Integrations
            </h3>
            <div class="space-y-3">
              <div class="card rounded-lg p-4">
                <strong class="block mb-1">Linear/JIRA</strong>
                <span class="text-sm opacity-80">Task management and issue tracking</span>
              </div>
              <div class="card rounded-lg p-4">
                <strong class="block mb-1">Slack</strong>
                <span class="text-sm opacity-80">Team communication and notifications</span>
              </div>
              <div class="card rounded-lg p-4">
                <strong class="block mb-1">Azure</strong>
                <span class="text-sm opacity-80">Cloud service management</span>
              </div>
              <div class="card rounded-lg p-4">
                <strong class="block mb-1">Database</strong>
                <span class="text-sm opacity-80">Direct query execution and schema management</span>
              </div>
            </div>
          </div>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-8">
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-4">Install MCP Server</h3>
            <div class="code-block rounded-lg p-4">
              <div class="text-xs opacity-60 mb-2">Installation</div>
              <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Install Linear MCP server</span>
npm install -g @linear/claude-mcp-server

<span class="opacity-60"># Install Database MCP server</span>
pipx install mcp-server-postgres

<span class="opacity-60"># Verify installation</span>
claude mcp list-servers</pre>
            </div>
          </div>
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-4">Usage Examples</h3>
            <div class="code-block rounded-lg p-4">
              <div class="text-xs opacity-60 mb-2">Commands</div>
              <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Query Linear issues</span>
"Show me all high priority bugs in the API project"

<span class="opacity-60"># Database operations</span>
"Get the top 10 customers by revenue this month"

<span class="opacity-60"># Azure resource management</span>
"List all VMs in production resource group"</pre>
            </div>
          </div>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <GlobeAltIcon class="w-5 h-5" />
              Open Standard Ecosystem
            </h3>
            <p class="text-sm opacity-80">MCP is rapidly becoming the open standard for AI agentic era. Growing adoption across development tools and platforms.</p>
          </div>
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <ShoppingBagIcon class="w-5 h-5" />
              Enterprise Adoption
            </h3>
            <p class="text-sm opacity-80">Expanding integration with enterprise tools and platforms. One-click server links, streaming transport, full tracing capabilities.</p>
          </div>
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
              <UserIcon class="w-5 h-5" />
              Token Management
            </h3>
            <p class="text-sm opacity-80">Claude Code manages large MCP outputs with 10K token warning threshold, configurable up to 25K tokens.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { WrenchScrewdriverIcon, CubeTransparentIcon, GlobeAltIcon, ShoppingBagIcon, UserIcon } from '@heroicons/vue/24/outline'
</script>