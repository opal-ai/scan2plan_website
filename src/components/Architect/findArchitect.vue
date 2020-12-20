<!--Version History--->
<!--
V1.0    Aditi     12/19/2020    Initial version
--->


<template>
    <div>
       <h1>FIND AN ARCHITECT</h1>
       <p>Let us know about your needs.</p>
       <div id="searchDetails">
           <div v-if="count === 0"> 
                <p> Where are you located? </p>
                <input type="text"/>
                <button class="bg-success nextButton" v-on:click="updateNext"> Next </button>
           </div>
            <div v-if="count === 1"> 
                <p> What services do you need?</p>
                <input type="text"/>
                <button class="bg-success nextButton" v-on:click="updateNext"> Next </button>
           </div>
            <div v-if="count === 2"> 
                <p> When do you need the architect?</p>
                <input type="text"/>
                <button class="bg-success nextButton" v-on:click="updateNext"> Next </button>
           </div>
           <div v-if="this.findingArchitect">
               Please wait... finding the best match..
           </div>
           <ArchitectList v-if="this.showArchitects"/>
       </div>
    </div>
</template>
<script>

import ArchitectList from './architectList'

export default {
    name: 'FindArchitect',
    components: {
        ArchitectList
    },
    data: function(){
        return {
            count : 0,
            findingArchitect: false,
            showArchitects: false
        }
    },
    methods : {
        updateNext : function(){
            this.count += 1;
            if(this.count === 3)
            {
                this.count = -1;
                this.findingArchitect = true
                setTimeout(() => {
                    console.log(this.showArchitects)
                    console.log("finding ? " + this.findingArchitect)
                    this.showArchitects = true
                    this.findingArchitect = false
                    console.log("show? " + this.showArchitects)
                } ,1000)
            }
        }
    }
}
</script>

<style scoped>
#searchDetails{
    margin-top: 15vh;
}

.nextButton{
    margin-left: 2vh;
}
</style>

