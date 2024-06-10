<template>
  <input
    type="text"
    :value="name"
    @input="$emit('update:name', $event.target.value)"
  />
  <!--$emit()-> name이 업데이트 될 때마다 벨류가 바뀐다.-->
</template>

<script>
export default {
  name: 'InputName',
  props: ['name'],
};
</script>
