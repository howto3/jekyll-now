---
layout: post
title: v-bind class binding
category: Vue.js
tags: [Vue.js, v-bind]
---


```javascript
<script src="https://cdnjs.cloudflare.com/ajax/libs/vue/1.0.24/vue.min.js"></script>


<div id="app">
  <label for="r1">Change colors</label><input type="checkbox" v-model="class1" id="r1">
  <br><br>
  <div v-bind:class="[class1 === 'ssss' ? 'class1' : 'class2']">
    directiva v-bind:class
  </div>
  <div v-bind:class="[class1 === 'yyyy' ? 'class1' : 'class2']">
    directiva v-bind:class
  </div>
  <div v-bind:class="[class1 === 'ssss' ? 'class1' : 'class2']">
    directiva v-bind:class
  </div>
  <div v-bind:class="[class1 === 'yyyy' ? 'class1' : 'class2']">
    directiva v-bind:class
  </div>
</div>


new Vue({
	el: '#app',
  data:{
  	class1: "yyyy"
  }
});

body{
  font-size: 1rem;
  font-family: arial;
}

.class1{
  background: red;
  color: yellow;
  float: left;
  clear:both;
}

.class2{
  background: green;
  color: blue;
  float: right;
 clear:both;
}
```
