<template lang="pug">
.block-component
  slot
</template>

<script>
export default {
};
</script>

<style lang="scss">
.block-component {
  transition: all 1s cubic-bezier(1, 0, 0, 1);
  .inner {
    padding: 12px 24px;
    padding-bottom: 24px;
    min-height: 32px;
    transition: all 1.25s cubic-bezier(1, 0, 0, 1);
  }
}
</style>
