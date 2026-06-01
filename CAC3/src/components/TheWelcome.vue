<script setup>
import WelcomeItem from './WelcomeItem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import GraphIcon from './icons/IconGraph.vue'
import FormIcon from './icons/IconForm.vue'
import CanadaIcon from './icons/IconCanada.vue'

const openReadmeInEditor = () => fetch('/__open-in-editor?file=README.md')
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <CanadaIcon />
    </template>
    <template #heading>
      <a 
      href="https://www.canada.ca/en/immigration-refugees-citizenship/services/canadian-citizenship/proof-citizenship/about.html" 
      target="_blank" 
      rel="noopener"
      >
        IRCC Documentation
      </a>
    </template>
     Official resources
    
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <FormIcon />
    </template>
    <template #heading>
      <RouterLink to="/submission">
        Application Data Submission
      </RouterLink>
    </template>

    Submit data for the tracker

  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <GraphIcon />
    </template>
    <template #heading>
      <RouterLink to="tracker">
        Application Data Tracker
      </RouterLink>
    </template>

    Analysis and visualizations of application data
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>
      <a href="https://www.reddit.com/r/Canadiancitizenship/" target="_blank" rel="noopener">
      Community
      </a>
    </template>

    Canadian citizenship community on Reddit
  </WelcomeItem>

  <!--
  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Support Vue</template>

    As an independent project, Vue relies on community backing for its sustainability. You can help
    us by
    <a href="https://vuejs.org/sponsor/" target="_blank" rel="noopener">becoming a sponsor</a>.
  </WelcomeItem>
  -->


</template>
