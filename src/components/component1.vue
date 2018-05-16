<template>
  <div class='component1'>
  <component2></component2>
  </div>
</template>

<script>
import component2 from './component2';

export default {
  name: 'component1',
  data() {
    return {
      msg: '',
    };
  },
  components: {
    component2,
  },
};
</script>
<style>
.component1{
	margin-left:400px;
	margin-top:100px;
	width:400px;
	height:460px;
	box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.6);
}
</style>
