<template>
    <li>
        <div>
            <header>
                <h3> {{ title }} </h3>
                <button>Supprimer</button>
            </header>
        </div>
        <p> {{ description }} </p>
        <nav>
            <a target="_blank" :href="link">Voir la ressource</a>
        </nav>
    </li>
</template>

<script>
export default {
    props : [
        'title',
        'description',
        'link'
    ]
}
</script>

<style scoped>
li {
  margin: auto;
  max-width: 40rem;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

h3 {
  font-size: 1.25rem;
  margin: 0.5rem 0;
}

p {
  margin: 0.5rem 0;
}

a {
  text-decoration: none;
  color: #42b983;
  font-weight: bolder;
}

a:hover,
a:active {
  color: teal;
}
</style>