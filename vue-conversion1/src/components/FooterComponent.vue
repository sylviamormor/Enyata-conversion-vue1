<script setup>

</script>

<template>
    <div class="footer">
        <div class="footnav">
            <div class="log">
                <img src="../assets/vectorfooter.png" class="fImage">
                <p class="footlog">Findtrend</p>
            </div>
            <div class="fLinks">
                <a href="" class="fItem">Privacy Policy</a>
                <a href="" class="fItem">Terms and Conditions</a>
                <a href="" class="fItem">Contact Us</a>
                <a href="" class="fItem">Careers</a>
            </div>
        </div>
    </div>
</template>

<style scoped>
.footer{
    padding: 10%;
}
.footnav{
    display: flex;
    flex-direction: column;
    gap: 30px;
    align-items: center;
}
.fImage{
    width: 40px;
    height: 40px;
}
.log{
    display: flex;
    gap: 20px;
    align-items: center;
}
.fLinks{
    display: flex;
    flex-direction: column;
    gap: 30px;
}
    .footlog{
        color: #000;
        text-align: center;
        font-size: 24px;
        font-style: normal;
        font-weight: 700;
        line-height: 24px;
    }
    .fItem{
        color: #000;
        text-align: center;
        font-size: 18px;
        font-style: normal;
        font-weight: 400;
        line-height: 18px;
        text-decoration: none;
    }
    @media (min-width: 900px){
        .footnav{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
    }
    .fLinks{
        display: flex;
        flex-direction: row;
        gap: 30px;
    }
    .footer{
        padding: 3%;
    }
    }
</style>