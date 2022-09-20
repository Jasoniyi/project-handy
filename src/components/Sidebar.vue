<template>
  <div class="sidebar-container">
    <div class="sidebar-wrapper">
      <ul>
        <li :key="link.id" v-for="link in links">
          <i :class="['fas', link.icon]"></i>
          {{ link.text}}
        </li>
      </ul>
    </div>
    
  </div>
</template>
<script>
import { Options, Vue } from 'vue-class-component';


@Options({
  components: {},
  data() {
    return {
      links: []
    }
  },
  created() {
    this.links = [
    {
      id: 1,
      icon: 'fa-home',
      text: 'Home'      
    },
    {
      id: 2,
      icon: 'fa-users',
      text: 'Clients'      
    },
    {
      id: 3,
      icon: 'fa-folder',
      text: 'Projects'      
    },
    {
      id: 4,
      icon: 'fa-file',
      text: 'Reports'      
    },
    ]
  }
})

export default class Sidebar extends Vue { }
</script>
<style>

  
.sidebar-container { 
    width: 20%;
    background-color: #163e52;
    color: #fff;
    height: 100vh;
  }
  
.sidebar-wrapper {
  padding:1em;
  display: flex;
}

.fas {
  padding-right: .6em;
}

li { 
  list-style: none;
  display: flex;
  padding: .7em 0;
  cursor: pointer;
}
</style>