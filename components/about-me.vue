<template>
  <div id="about">
    <div class="mb-2"><strong>About me:</strong></div>
    <div class="about">
      <div class="mr-4 mb-4 text-justify one">
        Working since 2014 on Software, I've been through every job on the
        field, from a ticket-grabbing developer, through full-stack,
        infrastructure, database management, continuous delivery, frontend and
        backend engineering, and even information security. <br />
        <br />
        I've managed teams of 1 to 15 people of various fields of expertise such
        as Design, Data Science, Quality Assurance and Engineering and I was
        quite lucky to work with some of the best in the business. <br />
        <br />
        Working directly with business owners and clients is something I have
        years of experience in, therefore I understand the value of translating
        a vision into an actionable roadmap and its features. <br />
        <br />
        Bringing you value is my passion, that's why I build stuff. <br />
      </div>
      <div class="two">
        <img
          src="~/assets/artur.jpg"
          class="border-2 border-blue-900 rounded-full"
        />
      </div>
    </div>
  </div>
</template>
<script lang="ts">
export default {
  name: 'AboutMe',
}
</script>
<style>
.about {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: space-between;
  align-items: center;

  @media (max-width: 625px) {
    display: block;
  }
}
.one {
  flex: 2 1 0;
  @media (max-width: 625px) {
    margin-right: 0;
  }
}

.two {
  flex: 1 1 0;
  width: 100%;
}

.two > img {
  max-width: 220px;
  margin: auto;
}
</style>