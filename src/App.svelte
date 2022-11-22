<script>
  import Header from './componentes/Header.svelte';
  import Dashboard from './componentes/Dashboard.svelte';


let notes = [
  {
    id: 0,
    title: 'Vacaciones',
    color: 'yellow',
    text: 'Hola!'
  },
  {
    id: 1,
    title: 'Vacaciones',
    color: 'red',
    text: 'Hola!'
  }
];
let copyNotes = [...notes];
let count = notes.length;
</script>

<main>
  <Header />
  <div>{count} notas</div>
  <Dashboard notes={notes} />
</main>

<style>
 
</style>
