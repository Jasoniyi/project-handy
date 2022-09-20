<template>
    <div class="dashboard-body">
        <div class="container">
            <div class="row">
                <div class="col-md-4">
                    <Card
                        title="Projects"
                        number="41"
                        description="Active Projects"
                    />
                </div>
                <div class="col-md-4">
                    <Card
                        title="Projects"
                        number="37"
                        description="Complete Projects"
                    />
                </div>
                <div class="col-md-4">
                    <Card
                        title="Projects"
                        number="4"
                        description="Incomplete Projects"
                    />
                </div>
        </div>

        <div class="dashboard-desc-row">
            <div class="row">
                    <div class="col-md-6">
                        <Card
                            title="Late and due milestones"
                            data="no data to be displayed"
                        />
                    </div>
                    <div class="col-md-6">
                        <Card
                            title="Top Clients"
                            data="no data to be displayed"
                        />
                    </div>
            </div>
         </div>
    </div>
    </div>
</template>
<script>

import { Options, Vue } from 'vue-class-component';
import Card from "../components/Card.vue"

@Options({
  components: {
     Card,
  },
})
export default class MyTask extends Vue {}
</script>

<style>
.dashboard-body {
    background-color: rgb(248, 246, 246);
    height: 100%;
    padding: 2em 2em;
}

.dashboard-desc-row {
    margin-top: 2em;
}
</style>