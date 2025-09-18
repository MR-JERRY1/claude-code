<template>
  <div class="slide absolute inset-0 flex items-center justify-center text-center">
    <div class="max-w-5xl mx-auto px-8 animate-fade-in">
      <h1 class="text-6xl font-bold mb-8 gradient-text tracking-tight">Claude Code</h1>
      <div class="card rounded-xl p-8 max-w-3xl mx-auto text-center">
        <p class="text-xl font-light opacity-90 leading-relaxed mb-6">
          AI-Powered Development Environment
        </p>
        <p class="text-sm opacity-70 leading-relaxed mb-6">
          Transform your development workflow with intelligent automation and context-aware assistance
        </p>
        <div class="flex justify-center gap-6 opacity-80 font-mono text-sm mb-8">
          <span>Smart Memory</span>
          <span>•</span>
          <span>AI Subagents</span>
          <span>•</span>
          <span>Custom Tools</span>
          <span>•</span>
          <span>GitHub Integration</span>
        </div>

        <div class="code-block rounded-lg p-4 text-left">
          <div class="text-xs opacity-60 mb-2">Quick Start</div>
          <pre class="text-sm opacity-80"><span class="opacity-60"># Option 1: Download from</span> <a href="https://nodejs.org/en/download" target="_blank" class="text-cyan-400 hover:text-cyan-300">https://nodejs.org/en/download</a>

<span class="opacity-60"># Option 2: Download and install nvm:</span>
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash
<span class="opacity-60"># in lieu of restarting the shell</span>
\. "$HOME/.nvm/nvm.sh"
<span class="opacity-60"># Download and install Node.js:</span>
nvm install 22

<span class="opacity-60"># Install Claude Code</span>
npm install -g @anthropic/claude-code

<span class="opacity-60"># Start coding with AI assistance</span>
claude "Add user authentication to my Vue app"</pre>
        </div>
      </div>
    </div>
  </div>
</template>