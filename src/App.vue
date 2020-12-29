<template>
  <div id="app">
    <Menu/>
    <Explore/>
    <About/>
    <Skills/>
    <WhatDo/>
    <Works/>
    <Contact/>
    <Foot/>
  </div>
</template>

<script>
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
import Explore from '@/components/Explore'
import Menu from '@/components/Menu'
import About from '@/components/About'
import Skills from '@/components/Skills'
import WhatDo from '@/components/WhatDo'
import Works from '@/components/Works'
import Contact from '@/components/Contact'
import Foot from '@/components/Foot'

export default {
  name: 'App',
  components:{
    Explore,
    Menu,
    About,
    Skills,
    WhatDo,
    Works,
    Contact,
    Foot
  }
}
</script>

<style>
#app {

}
</style>
