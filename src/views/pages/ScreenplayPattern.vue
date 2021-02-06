<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-12 col-md-6"
        v-for="framework in frameworks"
        :key="framework.title">
        <h4 class="text-center">{{ framework.title }}</h4>
        <div class="card mb-2">
          <div class="card-body">
            <ul>
              <li v-for="(item, index) in framework.list" :key="index">
                {{ item }}
              </li>
            </ul>
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
          title: 'Screenplay pattern',
          list: [
            'A technique that let you write better structured, more reusable, more maintainable and more readable tests.',
            'SerenityBDD makes It easy to apply',
            'Serenity package: DSL that helps you write more fluent tests in Java.',
            'Most of the things are already available within the framework where you need not to add external utilities for generating reports, logs',
            'Use narrative approach or Actor centric approach',
            'Actor – people who interact with the system or cause things to happen and observe the result',
            'An actor called it a name James',
            'An actor has abilities: James can browse the web'
          ]
        },
        
      ]
    }
  }
}
</script>