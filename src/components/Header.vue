<template>
  <header>
      <nav class="navbar navbar-expand-lg navbar-light bg-white">
        <div class="container p-3">
            <div class="my-nav d-flex justify-content-between">
                <div class="brand">
                <a class="navbar-brand" href="#">
                    <img src="../assets/dark-logo.png" alt="Max Coach" class="logo">
                </a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
            </div>
            <div class="collapse navbar-collapse d-flex" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li :key="index" v-for="(link,index) in links" class="nav-item dropdown">
                        <a class="nav-link color-link dropdown-toggle" :href="link.href" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                        {{link.name}}
                        </a>
                        <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                            <li :key="counter" v-for="(subl, counter) in link.sublink">
                                <a class="dropdown-item" :href="subl.href">{{subl.name}}</a>
                            </li>
                        </ul>
                    </li>
                </ul>
            </div>
            <div class="right d-flex">
                 <ul class="navbar-nav me-auto mb-2 mb-lg-0 d-flex align-items-center">
                    <img src="../assets/en.png" alt="" class="lingua">
                    <li class="nav-item dropdown">
                        <a class="nav-link color-link dropdown-toggle" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false"><strong>ENGLISH</strong></a>
                        <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                            <li>
                                <a class="dropdown-item" >
                                    <img src="../assets/fr.png" alt="" class="lingua">
                                    FRANCE
                                </a>
                            </li>
                            <li>
                                <a class="dropdown-item" >
                                    <img src="../assets/de.png" alt="" class="lingua">
                                    GERMAN
                                </a>
                            </li>
                        </ul>
                    </li>

                </ul>
                <form class="d-flex">
                    <input class="mysearch" type="search" placeholder="Search" aria-label="Search">
                    <button class="btn btn-outline-success" type="submit">Search</button>
                </form>
            </div>
            </div>
        </div>
    </nav>
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
@import "../assets/scss/partials/_variables.scss";
    header{
        font-family: $font;
        .logo{
            height: 30px;
        }
        .my-nav{
            gap: 100px;
            align-items: center;
        }
        nav{
            a{
                color: $tuna !important;
                font-size: 1.1em;
                font-weight: 400;
            }
        }
    }
</style>