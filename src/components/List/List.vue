<template>
  <div>
    <h1>Inputs</h1>
    <div>
      <div class="row">
        <div class="input-container">
          <Label text="<Input />" />
          <Input label="Label" placeholder="Placeholder" text="input" />
        </div>
        <div class="input-container">
          <Label class="grey" text="&:hover" />
          <Input label="Label" placeholder="Placeholder" text="input" />
        </div>
        <div class="input-container">
          <Label class="grey" text="&:focus" />
          <Input
            focus="focus"
            color="blue"
            label="Label"
            placeholder="Placeholder"
            text="input"
          />
        </div>
      </div>

      <div class="row">
        <div class="input-container">
          <Label text="<Input error />" />
          <Input error label="Label" placeholder="Placeholder" text="input" />
        </div>
        <div class="input-container">
          <Label class="grey" text="&:hover" />
          <Input label="Label" placeholder="Placeholder" text="input" />
        </div>
        <div class="input-container">
          <Label class="grey" text="&:focus" />
          <Input label="Label" error placeholder="Placeholder" text="input" />
        </div>
      </div>
      <div class="row">
        <div class="input-container">
          <Label text="<Input disabled />" />
          <Input
            disabled
            label="Label"
            placeholder="Placeholder"
            text="input"
          />
        </div>
      </div>

       <div class="row">
        <div class="input-container">
          <Label text="<Input helperText=”Some interesting text” />" />
          <Input label="Label" placeholder="Placeholder" text="input" helperText="Some interesting text" />
        </div>
        <div class="input-container">
          <Label text="<Input helperText=”Some interesting text error” />" />
          <Input error label="Label" placeholder="Placeholder" text="input" helperText="Some interesting text" />
        </div>
       
      </div>

        <div class="row">
        <div class="input-container col-6">
          <Label text="<Input startIcon />" />
          <Input  startIcon="telephone" label="Label" placeholder="Placeholder" text="input" helperText="Some interesting text" />
        </div>
        <div class="input-container col-6">
          <Label text="<Input endIcon />" />
          <Input endIcon="fingerprint" error label="Label" placeholder="Placeholder" helperText="Some interesting text" />
        </div>
       
      </div>

       <div class="row">
        <div class="input-container col-6">
          <Label text="<Input startIcon />" />
          <Input value="Text" label="Label" placeholder="Placeholder" />
        </div>
       
       
      </div>

       <div class="row">
        <div class="input-container col-6">
          <Label text="<Input size=”sm” />" />
          <Input size="sm" label="Label" placeholder="Placeholder" />
        </div>

         <div class="input-container col-6">
          <Label text="<Input size=”md” />" />
          <Input size="md" label="Label" placeholder="Placeholder" />
        </div>
       
       
      </div>

             <div class="row">
        <div class="input-container col-6">
          <Label text="<Input fullWidth />" />
          <Input fullWidth label="Label" placeholder="Placeholder" />
        </div>
             </div>

     <div class="row">
        <div class="input-container col-6">
          <Label text="<Input multiLine />" />
          <Input multiLine label="Label" placeholder="Placeholder" />
        </div>
        
       
       
      </div>

      
       
    </div>
  </div>
</template>

<script>
import Label from "./Label";
import Input from "../Input";
export default {
  name: "List",
  components: {
    Label,
    Input,
  },
};
</script>

<style src="./styles.css"></style>
