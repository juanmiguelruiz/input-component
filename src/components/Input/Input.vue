<template>
  <div>
    <label class="label" :class="[color, { red: error }]">{{ label }}</label>
    <div>
      <span class="material-icons start-icon">{{ startIcon }}</span>
      <input
        :class="[
          focus,
          size,
          variant,
          { error: error },
          { input__startIcon: startIcon },
          { input__fullWidth: fullWidth },
          { input__multiLine: multiLine }
        ]"
        :placeholder="placeholder"
        :value="value"
      />
      <span class="material-icons end-icon">{{ endIcon }}</span>
    </div>
    <label :class="[{ red: error }]" class="helper-text">{{
      helperText
    }}</label>
  </div>
</template>

<script>
export default {
  name: "Input",
  props: {
    color: {
      type: String,
      default: "",
      validator: function(value) {
        return ["blue", "red,", "grey"].indexOf(value) != -1;
      },
    },
    focus: {
      type: String,
      default: "",
    },
    helperText: {
      type: String,
      default: "",
    },
    placeholder: {
      type: String,
      default: "Placeholder",
    },
    label: {
      type: String,
      default: "label",
    },
    size: {
      type: String,
      default: "md",
      validator: function(value) {
        return ["sm", "md,", "lg"].indexOf(value) != -1;
      },
    },
    error: {
      type: Boolean,
      default: false,
    },

    multiLine: Boolean,
    fullWidth: Boolean,
    startIcon: String,
    endIcon: String,
   
   value: {
      type: String,
      default: "",
    },
  },
};
</script>

<style src="./styles.css"></style>
