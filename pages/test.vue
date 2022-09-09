<script>
    export default {
      name:'Test',
        async asyncData({ $axios }) {
          const ip = await $axios.$get('https://jsonplaceholder.typicode.com/todos/1')
          return { ip }
        },
      
      methods: {
       
      }
    }
  </script>
      
      <template>
        <h1>newdeal  {{ip}}</h1>
      </template>
          