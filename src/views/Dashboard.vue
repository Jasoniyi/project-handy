<template>
    <div class="dashboard-wrapper">
        <Sidebar />
        <div class="board">
            <Header />
            <MyTask />
        </div>
    </div>
</template>
<script>

import { Options, Vue } from 'vue-class-component';
import Sidebar from "../components/Sidebar.vue"
import Header from "../components/Header.vue"
import MyTask from "../components/MyTask.vue"

@Options({
  components: {
     Sidebar,
     Header,
     MyTask,
  },
})
export default class Dashboard extends Vue {}
</script>

<style>

/* body {
    background-color: #163e52;
} */

.dashboard-wrapper {
    /* width: 100vw; */
    display: flex;
}

.board {
    width: 100%;
}

</style>