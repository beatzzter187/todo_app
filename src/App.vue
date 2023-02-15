<script setup>
import TodoItem from "./components/TodoItem.vue";
// https://www.google.com/imgres?imgurl=https%3A%2F%2Fi.pinimg.com%2Foriginals%2Fc5%2F78%2F1d%2Fc5781d72c1298dc869b74702b4ee42a0.png&imgrefurl=https%3A%2F%2Fwww.pinterest.com%2Fpin%2F520869513146671442%2F&tbnid=PZkIWgyWGskinM&vet=12ahUKEwjIscTbs5L9AhUO47sIHd4hARkQMygBegUIARDDAQ..i&docid=MrqpUNS3WToXZM&w=800&h=600&q=todo%20website&client=firefox-b-e&ved=2ahUKEwjIscTbs5L9AhUO47sIHd4hARkQMygBegUIARDDAQ
</script>

<style>
.title {
  background-color: #6c39cb;
  text-align: center;
  font-size: 40px;
  font-weight: 800;
  font-style: initial;
  margin: 40px;
  margin-top: 70px;
  padding: 17px;
}
.input input {
  background-color: aqua;
  position: static;
  width: 10px;
  height: 5px;
}
</style>

<template>
  <div class="title rounded">
    <h3>Todo App</h3>
  </div>
  <div class="input">
    <input type="text" placeholder="test" />
  </div>
  <div class="grid place-items-center">
    <div
      class="bg-slate-200 border-slate-200 border-r border-b p-7 m-5 rounded w-1/2"
    >
      <div>
        <TodoItem>Dishes</TodoItem>
        <TodoItem>Dishes</TodoItem>
        <TodoItem>Dishes</TodoItem>
        <TodoItem>Dishes</TodoItem>
      </div>
      <div class="flex justify-center border-gray-700 mt-1">
        <button
          type="button"
          class="absolute inline-block px-10 py-2 bg-purple-600 text-white font-bold text-base leading-tight uppercase rounded shadow-md hover:bg-purple-700 hover:shadow-lg focus:bg-purple-700 focus:shadow-lg focus:outline-none focus:ring-0 active:bg-purple-800 active:shadow-lg transition duration-150 ease-in-out"
        >
          <p class="">+</p>
          New Task
        </button>
      </div>
    </div>
  </div>
</template>
