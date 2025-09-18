<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
    <div class="max-w-6xl w-full">
      <h2 class="text-3xl font-bold mb-6 text-center gradient-text">For Marketing Managers</h2>
      <p class="text-center opacity-80 mb-12 max-w-2xl mx-auto">Create campaigns that convert with AI-powered marketing automation</p>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <MegaphoneIcon class="w-5 h-5" />
            Campaign Automation
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Generate entire campaigns from brief. Create landing pages, email sequences, and ad copy that converts at scale.</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <ChartBarIcon class="w-5 h-5" />
            Data-Driven Insights
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Build custom analytics dashboards, automate A/B testing, and generate performance reports with actionable insights.</p>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-lg font-semibold mb-3 flex items-center gap-2">
            <GlobeAltIcon class="w-5 h-5" />
            SEO & Content
          </h3>
          <p class="text-sm opacity-80 leading-relaxed">Create SEO-optimized content at scale. Generate blog posts, social media content, and technical documentation instantly.</p>
        </div>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">Campaign Success Story</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">Product Launch Campaign</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Day 1: Strategy & Creation</span>
Input: Product specs, target audience
Generated: 50+ campaign variations
Time: <span class="text-green-400">2 hours vs 2 weeks</span>

<span class="opacity-60"># Day 2-7: Multi-Channel Launch</span>
• 10 landing pages (React + Next.js)
• 30 email templates (responsive)
• 100 social media posts
• 20 blog articles (SEO optimized)

<span class="opacity-60"># Week 1 Results</span>
Conversion rate: <span class="text-green-400">12% (3x industry avg)</span>
Lead quality: <span class="text-green-400">85% MQL rate</span>
Efficiency gain: <span class="text-green-400">60% faster execution</span>

<span class="opacity-60"># Month 1 Impact</span>
Reach: <span class="text-green-400">10x audience growth</span>
Engagement: <span class="text-green-400">5x interaction rate</span></pre>
          </div>
        </div>

        <div class="card rounded-lg p-6">
          <h3 class="text-xl font-semibold mb-4">Custom Slash Commands</h3>
          <div class="code-block rounded-lg p-4">
            <div class="text-xs opacity-60 mb-2">Example Marketing Commands You Can Create</div>
            <pre class="text-sm opacity-80 text-left"><span class="opacity-60"># Content generation</span>
claude /content "Q1 blog calendar"
→ 90 SEO articles, 500 social posts

<span class="opacity-60"># Landing page builder</span>
claude /landing "webinar registration"
→ A/B tested pages, 45% conversion

<span class="opacity-60"># Email automation</span>
claude /email-sequence "trial nurture"
→ 14-day drip, personalized content

<span class="opacity-60"># Analytics dashboard</span>
claude /dashboard "attribution model"
→ GA4 setup, Looker dashboards

<span class="opacity-60"># Competitive intel</span>
claude /compete-scan "market position"
→ SWOT analysis, positioning strategy

Efficiency: <span class="text-green-400">90% time saved</span>
Scale: <span class="text-green-400">10x content output</span></pre>
          </div>
        </div>
      </div>
    </div>
    </div>
  </div>
</template>

<script setup>
import { MegaphoneIcon, ChartBarIcon, GlobeAltIcon } from '@heroicons/vue/24/outline'
</script>