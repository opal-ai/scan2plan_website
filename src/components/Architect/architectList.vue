<template>
    <div>
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
                        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTsYVN1J0d02d7LIn3nJaXAF1b_LtE5Qk6X8g&usqp=CAU">
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