<template>
<div class="label-div">
  <label class="label">{{ text }}</label>
  </div>
</template>

<script>
export default {
  name: "Label",
  props: {
    text: {
      type: String,
      default: "",
    },
  },
};
</script>

<style>
.label {
  font-family: Ubuntu Mono;
font-style: normal;
font-weight: lighter;
font-size: 0.9em;
line-height: 12px;
color: #333333;
;
}

.label-div{
  margin-bottom: 8%;

}

.grey {
  color: #828282;
}
</style>
