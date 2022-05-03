<template>
  <div>
    
  <div class="center">
    <center>
   <h1>Welcome to the password generator</h1>
   <p>Get your password generated secured</p>
   <a id="projectlink" href="">Check the project!</a>
</center>
   <div class="container">
<h1 class="title">Password Generator</h1>
<h3 class="password-display" id="passwordDisplay">The password will appear here!</h3>
<form id="passwordGeneratorForm" class="form">
<label for="characterAmountNumber">Number Of Characters</label>
<div class="character-amount-container">
<input type="range" min="1" max="50" value="10" id="characterAmountRange">
<input class="number-input" type="number" min="1" max="50" value="10" id="characterAmountNumber">
</div>
<label for="includeNumbers">Include Numbers</label>
<input type="checkbox" id="includeNumbers">
<label for="includeSymbols">Include Symbols</label>
<input type="checkbox" id="includeSymbols">
<label for="includeUppercase">Include Uppercase <input type="checkbox" id="includeUppercase"> </label>
<button type="submit">Generate Password</button>
<a href="https://mihaidev.xyz/password-generator/how-to-protect.html">How to protect yourself more?</a>
<h2>Check how strength is the password generated</h2>
<iframe src="https://www.passwordmonster.com/" title="Iframe Example"></iframe>
</form>
</div>
</div>
  </div>
</template>

<style>
body {
  background: #49bd96;
  color: aliceblue;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  font-family: monospace;
}

#passwordDisplay {
  background: rgb(238, 229, 229);
  padding: 12px;
  border-radius: 2rem;
  border: #49bd96 2px solid;
}

#projectlink {
  text-decoration: underline;
   color: rgb(255, 255, 255);
   transition: 0.3s;
}

#projectlink:hover {
    color: rgb(196, 194, 194);
}


a {
  text-decoration: underline;
   color: rgb(42, 194, 123);
   transition: 0.3s;
}

a:hover {
   color: rgb(31, 153, 96);
}

.container {
  background-color: #d9d9db;
  box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.2);
  color: rgb(42, 194, 123);
   border: #49bd96 2px solid;
  padding: 20px;
  width: 370px;
  max-width: 100%;
  border-radius: 1rem;
  
}

.center {
  top: 50%;
  left: 50%;
  position: absolute;
  transform: translate(-50%, -50%);
}

</style>

<script>
  export default {
 
    mounted() {
      let passwordgeneratorscript = document.createElement('script')
      passwordgeneratorscript.setAttribute('src', 'password-config.js')
      document.head.appendChild(passwordgeneratorscript)
    },
   
  }
</script>

<script setup>
console.clear()
console.log("Created in nuxt.js and vue.js by Mihaidev-Cloud :3");
</script>