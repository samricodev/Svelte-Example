<script>
  import About from './components/About.svelte'
  import Text from './components/Text.svelte'
  import Person from './components/Person.svelte'
  import Skills from './components/Skills.svelte'

  const data = {
    name: "Sam",
    lastName: "Rico",
    age: 20
  }

</script>

<main>
  <h1>Mi primer sitio con Svelte</h1>
  <About />
  <Text anotherText="Hola hdtpm"/>
  <Text />
  <Person {...data}/>
  <Skills />
</main>

<style>
  :global(body){
    background-color: #f2eee2;
  }

  :global(:root){
    --theme-color: purple;
  }

  :global(body.darkMode){
    background-color: #1d3040;
    color: #bfc2c7;
  }

  h1{
    text-align: center;
  }

</style>