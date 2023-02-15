<script setup>
const todoName = "Dishes";
</script>
<style>
input {
  position: absolute;
  opacity: 0;
  height: 0;
  width: 0;
}
label {
  position: relative;
  display: block;
  padding-left: 30px;
  cursor: pointer;
}
label:before {
  content: "";
  position: absolute;
  top: 50%;
  margin-top: -10px;
  left: 0;
  display: block;
  height: 20px;
  width: 20px;
  background-color: #aa8aeb;
  border-radius: 3px;
}
label:hover:before {
  background-color: #be68da;
}
label:after {
  content: "";
  position: absolute;
  left: 7px;
  top: 1px;
  width: 5px;
  height: 10px;
  border: solid #333;
  border-width: 0 3px 3px 0;
  transform: rotate(45deg);
  opacity: 0;
}
input:checked + label:after {
  opacity: 1;
}
.todo {
  font-size: 20px;
  font-weight: 650;
}
</style>

<template>
  <input type="checkbox" id="checkbox" />
  <label for="checkbox" class="todo">{{ todoName }}</label>
  <p></p>
</template>
