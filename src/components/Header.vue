<template>
  <header>
      <ul>
          <li v-for="(link, index) in links" :key="index">
              <h1>{{link.name}}</h1>
              <ul>
                  <li v-for="(sub, counter) in link.sublink" :key="counter">
                      <h2>{{sub.name}}</h2>
                  </li>
              </ul>
          </li>
      </ul>
  </header>
</template>

<script>
export default {
    name: 'Header',
    data(){
        return{
            links: [
                {
                    "href": '#',
                    "name": 'Home',
                    sublink: [
                        {
                            "href": '#',
                            "name": 'Link1',
                        }
                    ]
                },
                {
                    "href": '#',
                    "name": 'Pages',
                    sublink: [
                        {
                            "href": '#',
                            "name": 'Link1',
                        }
                    ]
                },
                {
                    "href": '#',
                    "name": 'Courses',
                    sublink: [
                        {
                            "href": '#',
                            "name": 'Link1',
                        }
                    ]
                },
                {
                    "href": '#',
                    "name": 'Features',
                    sublink: [
                        {
                            "href": '#',
                            "name": 'Link1',
                        }
                    ]
                },
                {
                    "href": '#',
                    "name": 'Blog',
                    sublink: [
                        {
                            "href": '#',
                            "name": 'Link1',
                        }
                    ]
                },
                {
                    "href": '#',
                    "name": 'Shop',
                    sublink: [
                        {
                            "href": '#',
                            "name": 'Link1',
                        }
                    ]
                },     
            ]
        }
    },
}
</script>

<style lang="scss">
</style>