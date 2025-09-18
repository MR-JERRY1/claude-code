<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
      <div class="max-w-6xl w-full">
        <h2 class="text-3xl font-bold mb-12 text-center gradient-text">Competitive Landscape: AI CLI Tools 2024-2025</h2>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-8">
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-4">OpenAI Codex CLI</h3>
            <div class="space-y-3">
              <div class="text-sm opacity-80">
                <p class="mb-2"><strong>Key Features:</strong> Lightweight open-source coding agent, multimodal inputs (text, screenshots, diagrams), three approval modes (Read Only, Auto, Full Access)</p>
                <p class="mb-2"><strong>Models:</strong> GPT-5-Codex optimized for coding tasks, codex-mini-latest for efficient operations</p>
                <p><strong>Strengths:</strong> Zero-setup installation, local execution, ChatGPT plan integration</p>
              </div>
            </div>
          </div>

          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-4">Gemini CLI</h3>
            <div class="space-y-3">
              <div class="text-sm opacity-80">
                <p class="mb-2"><strong>Key Features:</strong> Open-source AI agent, 1M token context window, ReAct (Reason and Act) loop, Google Search grounding</p>
                <p class="mb-2"><strong>Integrations:</strong> VS Code, GitHub Actions, Zed editor, MCP support for custom extensions</p>
                <p><strong>Strengths:</strong> Generous free tier (60 req/min), multimodal capabilities with Veo and visual models</p>
              </div>
            </div>
          </div>

          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-4">Continue CLI</h3>
            <div class="space-y-3">
              <div class="text-sm opacity-80">
                <p class="mb-2"><strong>Key Features:</strong> Open-source modular coding agent, interactive and headless modes, permission system for AI actions</p>
                <p class="mb-2"><strong>Configuration:</strong> Uses config.yaml, supports custom models and tools, granular control with allow/ask/exclude flags</p>
                <p><strong>Strengths:</strong> Unix Philosophy scripting, same config as IDE extensions, customizable through Hub</p>
              </div>
            </div>
          </div>

          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-4">Goose (Block/GitHub)</h3>
            <div class="space-y-3">
              <div class="text-sm opacity-80">
                <p class="mb-2"><strong>Key Features:</strong> Extensible open-source AI agent, complete project generation from text prompts, browser automation capabilities</p>
                <p class="mb-2"><strong>Platforms:</strong> Desktop and CLI versions for macOS, Linux, Windows, web-based chat interface</p>
                <p><strong>Strengths:</strong> Plugin/extension system, multiple LLM provider integration, user-friendly project generation</p>
              </div>
            </div>
          </div>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-4">Market Trends 2024-2025</h3>
          <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
            <div>
              <h4 class="font-semibold mb-2">Context Management Revolution</h4>
              <p class="text-sm opacity-80">AI tools now handle 1M+ token context windows. Gemini CLI offers free 1M tokens, Claude Code provides enterprise-grade memory systems.</p>
            </div>
            <div>
              <h4 class="font-semibold mb-2">Multi-Model Support</h4>
              <p class="text-sm opacity-80">Tools support multiple AI models: GPT-4o, Claude 3.5 Sonnet, Gemini 2.0 Flash, with local model options via Ollama and other frameworks.</p>
            </div>
            <div>
              <h4 class="font-semibold mb-2">Agentic Workflows</h4>
              <p class="text-sm opacity-80">CLI agents now handle complex multi-step tasks: bug fixing, feature development, testing, deployment.</p>
            </div>
            <div>
              <h4 class="font-semibold mb-2">Enterprise Adoption</h4>
              <p class="text-sm opacity-80">Growing demand for enterprise features: security compliance, audit trails, team collaboration, and private model hosting.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
// No icons in this slide component
</script>
