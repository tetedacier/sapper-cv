<script>
import Title from '../components/Title.svelte'
import Contact from '../components/Rubric/contact.svelte'
import Presentation from '../components/Rubric/presentation.svelte'
import Skills from '../components/Rubric/skills.svelte'
import Trainings from '../components/Rubric/trainings.svelte'
import Experiences from '../components/Rubric/experiences.svelte'
</script>
<style>
main{
  display: flex;
}
aside {
  flex: 1;
  margin-right: 1em;
}

main>section {
  flex: 2;
}
aside .wrapper {
  padding: 0 1em 1em;
  background: #333333;
  border: 1px solid #333333;
  color: white;
}
</style>
<Title name="Fabien Jacq" />
<main>
  <aside>
    <div class="wrapper">
      <Contact />
      <Presentation />
    </div>
  </aside>
  <section>
    <Skills />
    <Trainings />
    <Experiences />
  </section>
</main>
