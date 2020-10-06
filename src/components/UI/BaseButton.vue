<template>
    <button :type="type" :class="mode">
        <slot></slot>
    </button>
</template>

<script>
export default {
    props : ['type', 'mode']
}
</script>

<style lang="less" scoped>
@vue-green : #42b983;

button {
  padding: 0.75rem 1.5rem;
  font-family: inherit;
  background-color: @vue-green;
  border: 1px solid @vue-green;
  color: white;
  cursor: pointer;

  &:hover, &:active {
    background-color: @vue-green;
  border-color: black;
  }
}



.flat {
  background-color: transparent;
  color: @vue-green;
  font-weight: 900;
  border: none;
}

.flat:hover,
.flat:active {
  background-color: lightgray;
}
</style>