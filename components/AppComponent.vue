// AppComponent.vue

<template>
	<div class="converter">
	  <h1 align="center">Currency Converter</h1>
	  <span >Enter Amount: </span><input type = "number" v-model.number = "amount" placeholder = "Enter Amount" /><br/><br/>
     <span>Convert From:</span>
     <select v-model = "convertfrom" style = "width:300px;font-size:25px;">
        <option v-for = "(a, index) in items"  v-bind:value = "a.name">{{a.desc}}</option>
     </select><br><br>
     <span>Convert To:</span>
     <select v-model = "convertto" style = "width:300px;font-size:25px;">
        <option v-for = "(a, index) in items" v-bind:value = "a.name">{{a.desc}}</option>
     </select><br/><br/>
     <span id = "display"> {{amount}} {{convertfrom}} equals {{finalamount}} {{convertto}}</span>
	</div>
</template>


// <script src = "vue_currency.js"></script>


<script>
   export default {

   }
</script>