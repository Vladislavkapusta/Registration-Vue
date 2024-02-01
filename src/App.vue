<script>
import Header from './components/Header.vue'
import Form from './components/Form.vue'
import Button from './UI/Button.vue'
import Info from './components/Info.vue'
export default{
  components:{
    Header, Form, Button, Info
  }
  
}

</script>

<template>
  <div class="body-layout">
      <Header></Header>
      <form>
    <div class="container">
      <Info></Info>
      <Form></Form>
      <Button></Button>
    </div>
      </form>

  </div>

</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,100;0,9..40,200;0,9..40,300;0,9..40,400;0,9..40,500;0,9..40,600;1,9..40,100;1,9..40,200;1,9..40,300;1,9..40,400;1,9..40,500&display=swap');

*{
  font-feature-settings: 'clig' off, 'liga' off;
  /* Headings/Typography Size 3 */
  font-family: "DM Sans";
}
.body-layout{
  display: flex;
  flex-direction: column;
}
.container{
  width: 700px;
  margin-top: 110px;
  margin-right: auto;
  margin-left: auto;

  display: flex;
  flex-direction: column;

  gap: 43px;
}
</style>
