<template>
    <div style="margin-top:5vh">
        <h2>3 Architects match your criteria.</h2>
        <b-container>
            <b-row id="resultRow">
                <b-col>
                    <div>
                        <p> <b>Moody H.</b><br>Experience: 2 years</p>
                        <img src="https://img.icons8.com/bubbles/2x/user-male.png">
                    </div>
                </b-col>
               <b-col>
                    <div>
                        <p> <b>Dino B.</b><br>Experience: 1 years</p>
                        <img src="https://img.icons8.com/bubbles/2x/manager.png">
                    </div>
                </b-col>
                <b-col>
                    <div>
                        <p> <b>Joanna M.</b><br>Experience: 2 years</p>
                        <img src="https://img.icons8.com/bubbles/2x/long-brown-curly-hair-lady-with-glasses.png">
                    </div>
                </b-col>
            </b-row>
        </b-container>
    </div>
</template>

<script>
export default {
    name: 'ArchitectList',
}
</script>

<style scoped>
    h2{
        color: #007bff;
    }
    #resultRow{
        margin-top: 4vh;
    }
</style>