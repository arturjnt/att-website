<template>
  <div id="how">
    <table>
      <thead>
        <tr>
          <th>How I Work</th>
          <th>Fields of Expertise</th>
          <th>Skills</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td class="pl-8 pr-2">
            <ol class="list-decimal">
              <li class="mb-4">
                We talk, so we can agree on a goal that brings you value.
              </li>
              <li class="mb-4">
                A step-by-step is drafted on what is necessary to achieve that
                goal.
              </li>
              <li class="mb-4">
                Payment either per project or hourly rate is agreed upon.
              </li>
            </ol>
          </td>
          <td>Web and Mobile Multiplatform iOS + Android</td>
          <Skills />
        </tr>
      </tbody>
    </table>
  </div>
</template>
<script lang="ts">
import Skills from './helpers/skills.vue'
export default {
  name: 'How',
  components: { Skills },
}
</script>

<style>
td,
th {
  @apply border-2 border-blue-900;
  padding: 5px 10px;
}

li > ul {
  margin-left: 50px;
}

@media (max-width: 625px) {
  /* Force table to not be like tables anymore */
  table,
  thead,
  tbody,
  th,
  td,
  tr {
    display: block;
  }

  #how {
    width: 100%;
  }

  thead tr {
    display: none;
  }

  td {
    /* Behave  like a "row" */
    position: relative;
    padding-left: 40% !important;
  }

  td:before {
    /* Now like a table header */
    position: absolute;
    /* Top/left values mimic padding */
    top: 6px;
    left: 6px;
    width: 35%;
    padding-right: 10px;
    white-space: nowrap;
  }

  td:nth-of-type(1) > ol {
    @apply list-inside;
  }
  td:nth-of-type(2) {
    border-top: none;
    border-bottom: none;
  }

  /*
	Label the data
	*/
  td:nth-of-type(1):before {
    content: 'How I Work';
    font-weight: bold;
  }
  td:nth-of-type(2):before {
    content: 'Fields of\a Expertise';
    white-space: pre;
    font-weight: bold;
  }
  td:nth-of-type(3):before {
    content: 'Skills';
    font-weight: bold;
  }
}
</style>