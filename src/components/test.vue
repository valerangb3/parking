<template>
  <div>
    <slot name="activator" :on="on" :otherSlotPropName="value" >
     
    </slot>
  </div>
</template>

<script>
export default {
data() {
    return {
      on: {
        click: console.log,
        contextmenu: console.log
      },
      value: "any key value pair"
    }
  }
}
</script>

<style>

</style>