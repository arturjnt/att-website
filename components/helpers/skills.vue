<template>
  <td>
    <Accordion title="Web">
      <ul class="list-disc list-inside">
        <li>HTML</li>
        <li>
          CSS
          <ul class="list-disc">
            <li>SASS</li>
          </ul>
        </li>
        <li>
          JavaScript
          <ul class="list-disc">
            <li>Node.js</li>
            <li>Vue.js</li>
          </ul>
        </li>
      </ul>
    </Accordion>
    <Accordion title="Mobile">
      <ul class="list-disc list-inside">
        <li>Dart</li>
        <li>Flutter</li>
      </ul></Accordion
    >
    <Accordion title="Infrastructure">
      <ul class="list-disc list-inside">
        <li>AWS (S3, EC2, etc)</li>
        <li>OVH (VPS)</li>
      </ul>
    </Accordion>
    <Accordion title="Continuous Deployment / Continuous Delivery">
      <ul class="list-disc list-inside">
        <li>Jenkins</li>
      </ul>
    </Accordion>
    <Accordion title="Database">
      <ul class="list-disc list-inside">
        <li>NoSQL</li>
        <li>SQL</li>
        <li>Firebase</li>
      </ul>
    </Accordion>
    <Accordion title="Management Tech">
      <ul class="list-disc list-inside">
        <li>Git</li>
        <li>JIRA</li>
        <li>Trello</li>
        <li>Miro</li>
        <li>ProductBoard</li>
        <li>Draw.io</li>
      </ul>
    </Accordion>
    <Accordion title="Security Advisory">
      <ul class="list-disc list-inside">
        <li>GDPR (DPIAs)</li>
        <li>ISO Certifications</li>
        <li>Pen-Testing</li>
        <li>Cookie law</li>
      </ul>
    </Accordion>
  </td>
</template>

<script lang="ts">
import Accordion from './accordion.vue'

export default {
  name: 'Skills',
  components: { Accordion },
}
</script>