<template>
    <StoredResources :resources="storedResources"/>
</template>

<script>
import StoredResources from './components/learning-resource/StoredResources'

export default {
    components : {
        StoredResources
    },
    data() {
        return {
            storedResources : [
                {
                    id : 'documentation',
                    title: 'Documentation',
                    description : 'La documentation officielle de Vue.js',
                    link : 'https://vuejs.org/'
                },
                {
                    id : 'google',
                    title: 'Google',
                    description : 'Demande à Google...',
                    link : 'https://www.google.fr/'
                }
            ]
        }
    },
}
</script>

<style >
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}
</style>