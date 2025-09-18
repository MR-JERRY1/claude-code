<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
      <div class="max-w-6xl w-full">
        <h2 class="text-3xl font-bold mb-12 text-center gradient-text">Agent Client Protocol (ACP)</h2>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3">Standardized Editor-Agent Communication</h3>
            <p class="text-sm opacity-80 leading-relaxed">ACP standardizes communication between code editors and coding agents that use generative AI to autonomously modify code.</p>
          </div>

          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3">Open Source & Interoperable</h3>
            <p class="text-sm opacity-80 leading-relaxed">Open source protocol with implementations in Rust and TypeScript. Enables interoperability between different coding tools and AI agents.</p>
          </div>

          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-3">Active Development & Community</h3>
            <p class="text-sm opacity-80 leading-relaxed">Protocol actively maturing through real-world implementations. Community-driven development with structured change process.</p>
          </div>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-6">
          <div class="card rounded-lg p-4">
            <h4 class="font-semibold mb-2">Editors</h4>
            <p class="text-sm opacity-80">Zed, Neovim, Marimo notebook</p>
          </div>
          <div class="card rounded-lg p-4">
            <h4 class="font-semibold mb-2">AI Agents</h4>
            <p class="text-sm opacity-80">Gemini, Claude Code</p>
          </div>
          <div class="card rounded-lg p-4">
            <h4 class="font-semibold mb-2">Languages</h4>
            <p class="text-sm opacity-80">Rust, TypeScript implementations</p>
          </div>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3">Technical Foundation</h3>
          <p class="text-sm opacity-80 leading-relaxed">Built on JSON Schema specifications with libraries for Rust and TypeScript. Provides consistent interface for AI-powered code modification across different tools and platforms.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
// No icons in this slide component
</script>
