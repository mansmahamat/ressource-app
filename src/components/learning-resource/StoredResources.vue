<template>
    <ul>
        <LearningResource v-for="resource in resources"
                            :key="resource.id"
                            :title="resource.title"
                            :description="resource.description"
                            :link="resource.link">

        </LearningResource>
    </ul>
</template>

<script>
import LearningResource from './LearningResource';

export default {
    props : ['resources'],
    components : {
        LearningResource
    }
}
</script>

<style lang="less" scoped>
ul {
  list-style: none;
  margin: 0;
  padding: 0;
  margin: auto;
  max-width: 40rem;
}
</style>