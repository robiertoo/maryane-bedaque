<script setup>
const courses = [
  {
    institution: 'Universidade Federal do Rio de Janeiro',
    completionDate: 'Dezembro de 2020',
    title: 'Bacharelado em Ciência da Computação',
    description:
      'Formação abrangente em desenvolvimento de software, algoritmos e estruturas de dados.',
  },
  {
    institution: 'Instituto de Tecnologia de São Paulo',
    completionDate: 'Junho de 2018',
    title: 'Análise e Desenvolvimento de Sistemas',
    description: 'Curso técnico com foco em desenvolvimento web e banco de dados.',
  },
  {
    institution: 'Universidade de São Paulo',
    completionDate: 'Março de 2023',
    title: 'Mestrado em Inteligência Artificial',
    description:
      'Pesquisa e desenvolvimento em áreas como aprendizado de máquina e processamento de linguagem natural.',
  },
  {
    institution: 'Senac',
    completionDate: 'Novembro de 2015',
    title: 'Técnico em Marketing Digital',
    description: 'Curso técnico com foco em estratégias de marketing online, redes sociais e SEO.',
  },
  {
    institution: 'Coursera',
    completionDate: 'Agosto de 2021',
    title: 'Especialização em Data Science',
    description:
      'Curso online com foco em análise de dados, machine learning e visualização de dados.',
  },
];
</script>

<template>
  <div class="flex flex-col md:flex-row md:space-x-4 space-y-2">
    <div class="w-full">
      <div class="mb-2">
        <h1>Formação</h1>
      </div>

      <div class="text-justify">
        <div v-for="course in courses" :key="course.institution">
          <h3>{{ course.institution }}</h3>
          <p>{{ course.completionDate }} - {{ course.title }}</p>
          <p>{{ course.description }}</p>
        </div>
      </div>
    </div>
  </div>
</template>
