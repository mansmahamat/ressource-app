<template>
    <header>
        <h1>
            {{ title }}
        </h1>
    </header>
</template>

<script>

export default {
    props : ['title']
}
</script>

<style lang="less" scoped>

@background : #42b983;
@text : white;

header {
  width: 100%;
  height: 5rem;
  background-color: @background;
  display: flex;
  justify-content: center;
  align-items: center;
  
  h1 {
  color: @text;
  margin: 0;
}

}


</style>