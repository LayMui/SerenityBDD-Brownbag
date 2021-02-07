<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-12 col-md-6"
        v-for="framework in frameworks"
        :key="framework.title">
        <h4 class="text-center headerText">{{ framework.title }}</h4>
        <div class="card mb-2">
          <div class="card-body">
            <p class=textColor> By putting the user interaction such as Click, enter text to the Task class or in another utility class routingUtility<p>
  
  
  
  <p class=codeSnippetText>@When("^(.*) login with username \"([^\"]*)\" and password \"([^\"]*)\"")
<p class=codeSnippetText>public void jamesLoginInWithUsernameAndPassword(String actor, String username, String password) {
{ </p>
	<span class="tab codeSnippetText">routingUtility.actorLogin(username, password);</span>
<p>}</p>
<div class="text-center">
    <img src="../../assets/image/actorlogin-code-snippet.png"/>
    <p class="header2Text">Task class: </p>
    <img src="../../assets/image/enterlogindetails-code-snippet.png"/>
    <p class="header2Text">Lean PageObject class: </p>
    <img src="../../assets/image/pageobject-code-snippet.png"/>
    <p class="header2Text">Example: </p>
    <img src="../../assets/image/how-to-make-stepdef-DSL.jpeg"/>
  </div>
    
        </div>
        </div>
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  data() {
    return {
      frameworks: [
        {
          title: 'To make the step definitions more readable using DSL',
         
        },
        
      ]
    }
  }
}
</script>


<style scoped>
.tab { 
       display:inline-block; 
       margin-left: 40px; 
     
}
.textColor {
   color: green;
}
.codeSnippetText {
   color: black;
   font-size: 12px;
}
.headerText {
   font-size: 20px;
   font-weight: bold;
   text-align: left;
   
}
.header2Text {
   font-size: 20px;
   font-weight: bold;
   text-align: left;
   color: orchid
}
</style>
