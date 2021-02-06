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
          title: 'The Value of SerenityBDD',
          list: [
            'Enable BDD style living documentation',
            'It has a defined PageObject class which hides WebDriver logic in “Page objects”.',
            'Most of the things are already available within the framework where you need not to add external utilities for generating reports, logs',
            'if you want to integrate web, mobile and api test, everything is available in one single framework',
            'Serenity BDD helps you write cleaner and more maintainable automated acceptance and regression tests faster.',
            'Screenplay pattern comes to the rescue 👍'
          ]
        },
        
      ]
    }
  }
}
</script>