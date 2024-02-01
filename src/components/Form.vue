<script>
import Input from '../UI/Input.vue'
export default{
    data(){
        return{
            Inputs:[
                    {name: 'Name', placehold: 'Your name', model: ''},
                    {name: 'Phone Number', placehold: '(123) 456 - 7890', model: ''},
                    {name: 'EMail', placehold: 'Your Mail ID', model: ''},
                    {name: 'Date', placehold: 'dd - mm - yyyy', model: ''}
            ]
            // ВРУЧНУЮ НАДО
        }
    },
    components:{
        Input
    }
}
</script>

<template>
    <div class="form-layout">
        <div class="form-container">
            <div class="form-info">
                <h3 class="form-title">
                    Contact details
                </h3>
                <p class="form-text">
                    Please fill your information so we can get in touch with you.
                </p>
            </div>
            <div class="inputs-layout">
                        <p class="input-title">Name</p>
                        <Input placehold="Your Name" model=''></Input>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .input-title{
        color: var(--Neutral-800, #170F49);
        font-feature-settings: 'clig' off, 'liga' off;
        /* Other/18-20 M */
        font-family: "DM Sans";
        font-size: 18px;
        font-style: normal;
        font-weight: 500;
        line-height: 20px; /* 111.111% */
    }
    .form-title{
        color: var(--Neutral-800, #170F49);
        font-feature-settings: 'clig' off, 'liga' off;
        font-family: "DM Sans";
        font-size: 24px;
        font-style: normal;
        font-weight: 700;
        line-height: 35px; /* 145.833% */

        margin: 0;
    }
    .form-text{
        color: #6F6C90;
        font-feature-settings: 'clig' off, 'liga' off;
        font-family: "DM Sans";
        font-size: 18px;
        font-style: normal;
        font-weight: 500;
        line-height: 30px; /* 166.667% */

        margin: 0;
    }
    .form-info{
        display: flex;
        flex-direction: column;

        gap: 6px;

        border-bottom: #D9DBE9 1px solid;

        padding-bottom: 16px;
    }
    .form-layout{
        border-radius: 34px;
        border: 1px solid #EFF0F6;

        background: #FAF8F8;

        /* Cards/Short Default */
        box-shadow: 0px 5px 16px 0px rgba(8, 15, 52, 0.06);
    }
    .form-container{
        width: 600px;
        margin-top: 25px;
        margin-right: auto;
        margin-left: auto;

        display: flex;
        flex-direction: column;

        gap: 43px;
}
</style>