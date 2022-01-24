<template>
  <header>1</header>
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