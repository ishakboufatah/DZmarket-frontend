<template>
  <div class="navbar">
    <router-link to="/" class="Dz_market">
      <span class="DZ">DZ</span>
      <span class="space"> &nbsp;</span>
      <span class="market" >market</span>
		</router-link>
    <router-link to="/cart" class="Buy" ></router-link>
    <div class="GroupResearch">
      <div class="Research">
        <div class="Research_Rectangle"></div>
        <div class="risearch-line" >
          <img class="Vector" src="../assets/Vector.svg"/>
        </div>
        

      </div>
      <select class="navbar-list" v-model="selectedValue">
      <option v-for="listValue in valuesList" v-bind:key="listValue" :value="listValue.value">
            {{listValue.text}}
        </option>
        
        
      </select>
      
    </div>
     
    

    
  </div>
<router-view/>
</template>

<script>
export default {
  name: "NavBar",
  props: {
    
    
  },
  data() {
        return {
        selectedValue: '1',
        valuesList: [
      { text: 'All', value: '1' },
      { text: 'Beauty', value: '2' },
      { text: 'Women’s clothing', value: '3' },
      { text: 'Video Games', value: '4' },
      { text: 'Toys & Games', value: '5' },
      { text: 'Sports', value: '6' },
      { text: 'Software', value: '7' },
      { text: 'Movies', value: '8' },
      { text: 'Girl’s Fashion', value: '9' },
      { text: 'Men’s Fashion', value: '10' },
      { text: 'Computers', value: '11' },
      { text: 'Electronics', value: '12' },
      { text: 'Books', value: '13' },
      

    ]
        }
    }
};
</script>

<style >
@font-face {
  font-family: "Rancho";
  src: local("Rancho"),   url(/public/fonts/Rancho/Rancho-Regular.ttf) format("truetype");
}
.navbar{
position: absolute;
height: 70px;
left: 0px;
right: 0px;
top: 0px;

background: rgba(0, 0, 0, 0.18);
box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}
.Dz_market{
position: absolute;
width: 209px;
height: 52px;
left: 42px;
top: 5px;

font-family: 'Rancho';
font-style: normal;
font-weight: 400;
font-size: 35px;
line-height: 43px;
display: flex;
align-items: center;
text-decoration:NONE;

color: #000000;
}
.DZ{
font-family: 'Rancho';
font-style: normal;
font-weight: 400;
font-size: 35px;
line-height: 43px;
display: flex;
align-items: center;



color: #000000;
}
.space{
font-family: 'Roboto';
font-style: normal;
font-weight: 700;
font-size: 35px;
line-height: 41px;
display: flex;
align-items: center;

color: #000000;
}
.market{
font-family: 'Rouge Script';
font-style: normal;
font-weight: 400;
font-size: 35px;
line-height: 41px;
display: flex;
align-items: center;

color: #000000;

}
.Buy{
position: absolute;
width: 30px;
right: 221px;
top: 34.29%;
bottom: 22.86%;

background: url(../assets/Buy.png);  
}
.GroupResearch{
position: absolute;
height: 42px;
left: 260px;
right: 339px;
top: 14px;

background: #FFFFFF;
box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
border-radius: 5px;


}
.Research{
position: absolute;
width: 60px;
height: 42px;
right: 00px;
top: 0px;
border-radius: 5px;
}

.risearch-line{
position: absolute;
height: 24px;
left: 18px;
right: 18px;

bottom:9px;
}
.Vector{
position: absolute;
left: 8.33%;
right: 7.03%;
top: 8.33%;
bottom: 7.03%;


}
.Research_Rectangle{
position: absolute;
width: 60px;
height: 42px;
right: 0px;
bottom: 0px;

background: rgba(251, 115, 17, 0.67);
border-radius: 0px 5px 5px 0px;
}
.navbar-list{
position: absolute;
left: 00px;
width: 60px;
top: 0px;
bottom: 0px;
Border: none;
border-radius: 5px 0px 0px 5px;
}
.Rectangle_3{
position: absolute;
left: 00px;
width: 60px;
top: 0px;
bottom: 0px;
background: rgba(196, 196, 196, 0.33);
border-radius: 5px 0px 0px 5px;
}

</style>