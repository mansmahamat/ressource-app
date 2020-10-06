<template>
    <li>
        <base-card>
            <header>
                <h3> {{ title }} </h3>
                <base-button mode="flat" >Supprimer</base-button>
            </header>
            <p> {{ description }} </p>
            <nav>
              <a target="_blank" :href="link">Voir la ressource</a>
            </nav>
        </base-card>
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


<style lang="less" scoped>
@link-color : #42b983;
@link-hover : teal;
@margin-top : 0.5rem 0;

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
  margin: @margin-top;
}

p {
  margin: @margin-top;
}

a {
  text-decoration: none;
  color: @link-color;
  font-weight: bolder;
  &:hover {
    color: @link-hover;
  }
}


</style>