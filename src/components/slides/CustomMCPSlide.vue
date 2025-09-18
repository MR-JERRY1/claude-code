<template>
  <div class="slide absolute inset-0">
    <div class="flex items-center justify-center min-h-screen p-8">
      <div class="max-w-6xl w-full">
        <h2 class="text-3xl font-bold mb-12 text-center gradient-text">Why Build Custom In-House MCP Servers?</h2>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-8">
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-4 flex items-center gap-2">
              <CircleStackIcon class="w-5 h-5" />
              Proprietary Data Access
            </h3>
            <p class="text-sm opacity-80 leading-relaxed mb-4">Connect Claude Code directly to your internal systems, databases, and APIs that contain your most valuable business data.</p>
            <div class="space-y-2">
              <p class="text-sm opacity-80"><strong>Internal APIs:</strong> Customer databases, inventory systems, financial records</p>
              <p class="text-sm opacity-80"><strong>Legacy Systems:</strong> Mainframe data, custom databases, proprietary formats</p>
              <p class="text-sm opacity-80"><strong>Real-time Data:</strong> Live metrics, operational dashboards, monitoring systems</p>
            </div>
          </div>

          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-4 flex items-center gap-2">
              <CheckCircleIcon class="w-5 h-5" />
              Competitive Advantage
            </h3>
            <p class="text-sm opacity-80 leading-relaxed mb-4">Generic tools can't understand your unique business processes. Custom MCP servers give Claude Code deep context about your organization.</p>
            <div class="space-y-2">
              <p class="text-sm opacity-80"><strong>Business Logic:</strong> Your specific workflows, approval processes, domain knowledge</p>
              <p class="text-sm opacity-80"><strong>Industry Expertise:</strong> Regulatory requirements, compliance rules, best practices</p>
              <p class="text-sm opacity-80"><strong>Institutional Knowledge:</strong> Years of accumulated wisdom baked into AI workflows</p>
            </div>
          </div>
        </div>

        <div class="space-y-6">
          <div class="card rounded-lg p-6">
            <h3 class="text-lg font-semibold mb-4 flex items-center gap-2">
              <LockClosedIcon class="w-5 h-5" />
              Security & Control
            </h3>
            <p class="text-sm opacity-80 leading-relaxed mb-4">Keep sensitive data within your infrastructure while gaining AI capabilities. Full control over access, authentication, and data flow.</p>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
              <div>
                <h4 class="font-semibold mb-2">On-Premise Deployment</h4>
                <p class="text-sm opacity-80">Data never leaves your network. Deploy MCP servers behind your firewall with complete isolation.</p>
              </div>
              <div>
                <h4 class="font-semibold mb-2">Custom Authentication</h4>
                <p class="text-sm opacity-80">Integrate with your existing SSO, LDAP, or custom auth systems. Role-based access controls.</p>
              </div>
              <div>
                <h4 class="font-semibold mb-2">Audit & Compliance</h4>
                <p class="text-sm opacity-80">Full audit trails, compliance reporting, and data governance aligned with your policies.</p>
              </div>
            </div>
          </div>

          <div class="card rounded-lg p-6 mb-8">
            <h3 class="text-lg font-semibold mb-4 flex items-center gap-2">
              <RocketLaunchIcon class="w-5 h-5" />
              Implementation Strategy
            </h3>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
              <div>
                <h4 class="font-semibold mb-2">Start Simple</h4>
                <p class="text-sm opacity-80">Begin with read-only database queries or API endpoints. Python/TypeScript SDKs make development straightforward.</p>
              </div>
              <div>
                <h4 class="font-semibold mb-2">Scale Gradually</h4>
                <p class="text-sm opacity-80">Add write operations, complex workflows, and multi-system integrations as confidence grows.</p>
              </div>
              <div>
                <h4 class="font-semibold mb-2">Enterprise Ready</h4>
                <p class="text-sm opacity-80">Built-in load balancing, failover, and monitoring. Deploy as microservices or serverless functions.</p>
              </div>
            </div>
          </div>

        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { CircleStackIcon, CheckCircleIcon, LockClosedIcon, RocketLaunchIcon } from '@heroicons/vue/24/outline'
</script>
