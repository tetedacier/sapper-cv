<script>
import Title from '../components/Title.svelte'
import Contact from '../components/Rubric/contact.svelte'
import Presentation from '../components/Rubric/presentation.svelte'
import Skills from '../components/Rubric/skills.svelte'
import Trainings from '../components/Rubric/trainings.svelte'
import Experiences from '../components/Rubric/experiences.svelte'
</script>
<style>
.layout{
  display: flex;
}

.personal-information {
  flex: 1;
  margin-right: 1em;
}

.personal-information .wrapper {
  padding: 0 1em 1em;
  background: #333333;
  border: 1px solid #333333;
  color: white;
}

.curriculum {
  flex: 2;
}
</style>
<svelte:head>
  <title>Curriculum vitæ de Fabien Jacq</title>
  <meta name="description" content="Curriculum vitæ de Fabien Jacq" />
</svelte:head>
<Title name="Fabien Jacq" />
<section class="layout">
  <section class="personal-information">
    <div class="wrapper">
      <Contact />
      <Presentation />
    </div>
  </section>
  <section class="curriculum">
    <Experiences />
    <Skills />
    <Trainings />
  </section>
</section>
