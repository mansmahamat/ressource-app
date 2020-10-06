<template>
    <TheHeader title="Ressources"/>
</template>

<script>
import TheHeader from './components/layouts/TheHeader';

export default {
    
    components : {
        TheHeader
    },
    data() {
        return {
            storedResources : [
                {
                    id : 'documentation',
                    title: 'Documentation',
                    description : 'La documentation officielle de Vue.js 3',
                    link : 'https://v3.vuejs.org/'
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