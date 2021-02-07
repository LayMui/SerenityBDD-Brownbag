<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-12 col-md-6"
        v-for="framework in frameworks"
        :key="framework.title">
        <h4 class="text-center">{{ framework.title }}</h4>
        <div class="card mb-2">
          <div class="card-body">
            <p> theActorCalled(actor)
               <span class="tab">should(
                        <p class=textColor>eventually</p>(seeThat(the(GoalPage.addNewGoalButton),  <p class=textColor>isVisible()</p>)));
   </span></p>
   <p>
   theActorInTheSpotlight().attemptsTo(Add.newGoal());
  </p>

  
  
  <p>public class Add {
    <span class=tab>public static Performable newGoal() {
        return Task.where(
                "{0} attempts to add new goal",
                <p class=textColor>Click.on(GoalPage.addNewGoalButton));</p>

    }
    
    </span>
} </p>
          </div>
        </div>
      </div>
    </div>
    <p class="left">
      Reference: <a href="https://groups.google.com/g/thucydides-users/c/zxvX6TZCbNs?pli=1" target="_blank">https://groups.google.com/g/thucydides-users/c/zxvX6TZCbNs?pli=1
</a>
<p>theActorCalled("Mary").should(eventually(seeThat(the(LoginPage.signInButton), isVisible())).waitingForNoLongerThan(30).seconds());
      </p>
<p>This will not fail if the matcher cannot be evaluated the first time, but will retry up to a maximum of 'serenity.timouts' seconds (5 by default).</p>
  
   <p class=subHeadingColor>Using the Awaitility framework</p>
   <p> Awaitility.with().pollInSameThread().await().atMost(60,TimeUnit.SECONDS).untilAsserted(
            () -> theActorCalled("Mary").should(eventually(seeThat(the(LoginPage.signInButton), isVisible()))));
       </p>

  </div>
</template>

<script>
export default {
  data() {
    return {
      frameworks: [
        {
          title: 'How to prevent flakiness',
         
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
   color: blue;
}
.subHeadingColor {
  color: red;
  font-size: 20px;
   text-decoration: underline overline;
}
</style>
