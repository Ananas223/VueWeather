<template>
    <div class="informer-container">
        <InformerTemperature/>
        <FlexBreak/>
        <InformerHumidity/>
        <VerticalDivider/>
        <InformerWind/>
    </div>
</template>
<script>
import InformerTemperature from './Temperature.vue'
import FlexBreak from './FlexBreak.vue'
import InformerHumidity from './Humidity.vue'
import VerticalDivider from './VerticalDivider.vue'
import InformerWind from './Wind.vue'

export default{
  name: 'InformerContainer',
  components: {
    InformerTemperature,
    FlexBreak,
    InformerHumidity,
    InformerWind,
    VerticalDivider
  }
}
</script>
<style>
.informer-container {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  flex-wrap: wrap;
  width: 400px;
  min-height: 255px;
  padding: 30px;
  background-image: url('../assets/img/forest.png');
  background-size: cover;
  background-position: center center;
  border-radius: 20px;
  box-shadow: 0px 0px 10px 0px rgba(50, 50, 50, 0.75);
}
</style>