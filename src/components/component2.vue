<template>
<div>
  <div class='component2'>
  <form>
  <form-group>
  <label for='user'>Username</label>
  <input type='text' name='user' class='txtbox' v-model='username'>
  </form-group>
  <br>
  <form-group>
  <label for='email'>Email</label>
  <input type='email' name='email' class='txtbox' v-model='email'>
  </form-group>
  <br>
  <form-group>
  <label for='dob'>Date of Birth</label>
  <input type='date' name="dob" class='txtbox' v-model='dob'>
  </form-group><br>
  <form-group>
  <label for='mobile'>Mobile</label>
  <input type='tel' name='mobile' class='txtbox' v-model='number'>
  </form-group>
  </form>
  </div>
  <br>
  <div class='component3'>
  <component3 :username='username' :email='email' :dob='dob' :number='number'></component3>
  </div>
  </div>
</template>

<script>
import component3 from './component3';

export default {
  name: 'component2',
  data() {
    return {
      username: '',
      email: '',
      dob: '',
      number: '',
    };
  },
  components: {
    component3,
  },
};
</script>

<style>
body {
    margin:50px 30px;
}
label,input {
padding:5px;
 display: block;
 width: 200px;
 height: 22px;
 float: left;
 margin-bottom: 10px;
 border: none;
}
.txtbox{
	border-bottom: 1px solid black;
}
label {
 text-align: right;
 width: 100px;
 padding-right: 30px;
}

br {
 clear: left;
}
.component2{
	margin: 10px;
	height: 200px;
	box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.6);
}
.component3{
margin:10px;
height:200px;
	box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.6);
}
</style>
