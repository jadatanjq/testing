<!-- <template>
    <div v-if="isSelected">
        <slot></slot>
    </div>
</template>

<script>
    export default {
    props: {
        isSelected: {
        type: Boolean,
        },
    },
    }
</script>
   -->

<template>
<div class='tab' v-show='isActive'>
  <slot></slot>
</div>
</template>
  
<script>
export default {
  props: {
    title: {
      type: String,
      default: 'Tab'
    }
  },
  
  data () {
    return {
      isActive: true
    }
  }
}
</script>
