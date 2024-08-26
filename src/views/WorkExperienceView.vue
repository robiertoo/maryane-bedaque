<script setup>
const experiences = [
  {
    "position": "Full Stack Developer",
    "description": "Web application development using technologies such as React, Node.js, and MongoDB.",
    "city": "São Paulo",
    "state": "SP",
    "workExperience": "3 years"
  },
  {
    "position": "Digital Marketing Analyst",
    "description": "Creation and management of online campaigns, data analysis, and results optimization.",
    "city": "Belo Horizonte",
    "state": "MG",
    "workExperience": "2 years and 6 months"
  },
  {
    "position": "Project Manager",
    "description": "Planning, execution, and monitoring of projects, team management, and alignment with stakeholders.",
    "city": "Porto Alegre",
    "state": "RS",
    "workExperience": "5 years"
  },
  {
    "position": "Graphic Designer",
    "description": "Creation of graphic pieces for various platforms, visual identity, and development of marketing materials.",
    "city": "Recife",
    "state": "PE",
    "workExperience": "1 year and 9 months"
  },
  {
    "position": "Sales Consultant",
    "description": "Prospecting and customer service, negotiation, and sales closing.",
    "city": "Curitiba",
    "state": "PR",
    "workExperience": "4 years"
  }
];
</script>

<template>
  <div class="flex flex-col md:flex-row md:space-x-4 space-y-2">
    <div class="w-full">
      <div class="mb-2">
        <h1>Experiências profissionais</h1>
      </div>

      <div class="text-justify">
        <div v-for="experience in experiences" :key="experience.position">
          <h3>{{ experience.position }}</h3>
          <p>{{ experience.description }}</p>
          <p>{{ experience.city }}, {{ experience.state }} - {{ experience.workExperience }}</p>
        </div>
      </div>
    </div>
  </div>
</template>
