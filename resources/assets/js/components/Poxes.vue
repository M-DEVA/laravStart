<style>
.alfabetBox {
  display: none;
}

input[type=text] 
{
border: none;
  border-bottom: 2px solid rgb(0, 0, 0);
  /* background-color:#f2f3f8 ; */
  margin-left: 30px;
 
}
input[type=radio]{
margin-left: 100px;
}
.facing{
    color:white;
    background-color: blue;

}
.card-body{
    background-color:#f2f3f8;
}

fieldset
{
display: block;
  margin-left: 2px;
  margin-right: 2px;
  padding-top: 0.35em;
  padding-bottom: 0.625em;
  padding-left: 0.75em;
  padding-right: 0.75em;
  border: 5px groove (internal value);
  border-width: 6px;
  background-color: white;
   /*width:100%; */
  
}
.left{
  float: left; 
  width: 60%;
}
.right{
  float: right;
  width: 40%;
}


.submit{float:right;
  border-radius:5px;
  width:150px;
  background-color:#ff9933;
  font-family:serif;

}


.cancel{float:left;
  margin-left:100px;
  border-radius:5px;
  width:150px;
  background-color:#c7c7c7; 

}
</style>

<template>
    <div class="container">
      

                  
                    <form action="">
                      <div class="left">
                        <i class="fa fa-arrow-left fa-2x"></i> <label style="font-size:30px;padding-left: 19px"> Add Poxes </label>
                        <fieldset>
                        <label for="pname">Enter Property Name:</label>
                         <input type="text" id="pname" name="pname">
                         <br>
                           
                       <label for="pname">Select Property Type:</label>
                       <div>
                       <label><input type="radio" name="alfabet" class="click" value="flat" id="flat"> FLAT </label>
                       <label><input type="radio" name="alfabet" class="click" value="plot" id="plot"> PLOT</label>
                       <label><input type="radio" name="alfabet" class="click" value="estab" id="estab"> ESTAB </label>
                       </div>
                       </fieldset>
                       <br>
                                         <div class="A alfabetBox ">
                                           <fieldset>

                     <label for="">Select Room Config</label>
                     <div >
                   <label><input type="radio" name="alfabet1"  value="1BHK" > 1BHK</label>
                   <label><input type="radio" name="alfabet1"  value="2BHK" > 2BHK </label>
                   <label><input type="radio" name="alfabet1"  value="3BHK" >3BHK</label>
                   </div>
            <label for="floor-no">Enter Floor No:</label>
            <input type="text" id="floor-no" name="floorno">
            <br>
             <label for="cars">Select Facing Type:</label>
    <select name="facing" id="facing-type" class="facing">
     <option value="north">North</option>
     <option value="south">South</option>
     <option value="east">East</option>
     <option value="west">West</option>
     <option value="north">North-East</option>
     <option value="south-east">South-East</option>
     <option value="south-west">South-West</option>
    </select>
  <br>
   <label for="floor-no">Enter Builtup Area:</label>
            <input type="text" id="Barea" name="builtarea">Sq Ft <br>
             <div>
              <label><input type="radio" name="alfabet2"  id="rent" value="rent"> Rent</label>
             <label><input type="radio" name="alfabet2" id="sale"  value="sale"> Sale </label>
           </div>

  </fieldset>
       </div>
     
      <!-- <br> -->
    
         <div class="rent alfabetBox">
           <fieldset>

               <label for="rent-value">Rent:</label>
                         <input type="text" id="rent-value" name="rent-value" />
               <label for="deposit-value">Deposit:</label>
                         <input type="text" id="deposit-value" name="deposit-value" />
</fieldset>
<br>
<fieldset>
<label for="deposit-value">Enter Contact Name:</label>
                         <input type="text" id="contact-Name" name="contact-name">
                         <br>
<label for="deposit-value">Enter Contact Number:</label>
                         <input type="text" id="contact-number" name="contact-number">
                         
 </fieldset>
         </div>
        

         <div class="sale alfabetBox">
            <fieldset>
        
          <label for="cost-value">Enter Selling Cost:</label>
                         <input type="text" id="cost-value" name="cost-value">
<br>        <label for="deposit-value">Enter Contact Name:</label>
                         <input type="text" id="contact-Name" name="contact-name">
                         <br>
<label for="deposit-value">Enter Contact Number:</label>
                         <input type="text" id="contact-number" name="contact-number">
                         
 </fieldset>
         </div>
        
<div class="B alfabetBox">
<fieldset>
<label for="plot-type">Select Plot Type: </label>
<div>
<label for=""><input type="radio" name="plot-type" value="residential"> Residential</label>
<label for=""><input type="radio" name="plot-type" value="commercial"> Commercial</label>
<label for=""><input type="radio" name="plot-type" value="agricultural">Agricultural</label>
</div>  
<label for="">Enter Plot Area:</label>
<input type="text" name="plot-area"> <label>Sq Ft</label><br>
<label for="">Select:</label>
<label for=""><input type="radio" name="plot-type1" value="sale" id="plot-sale">Sale</label>
<label for=""><input type="radio" name="plot-type1" value="lease" id="plot-lease">Lease</label>
</fieldset>

</div>
<br>
<div class="plot-sale alfabetBox">
<fieldset>
<label for="">Enter Selling cost:</label>
<input type="text" name="sell-cost">
</fieldset>

</div>
<div class="plot-sale alfabetBox">
<fieldset>
<label for="">Enter Contact Name:</label>
<input type="text" name="pcontact_name"><br>
<label for="">Enter Contact Number:</label>
<input type="text" name="pcontact_number">
</fieldset>

</div>
<div class="plot-lease alfabetBox">
<fieldset>
<label for="">Enter Lease Amount:</label>
<input type="text" name="lease-amount">
<br>
<label for="">Enter Lease Period:</label>
<input type="text" name="lease-period">
<br>
<label for="">Enter Contact Name:</label>
<input type="text" name="lcontact-name">
<!-- <br>
<label for=""></label> -->
    </fieldset>

  </div>


<div class="C alfabetBox">
<fieldset>
  <label for="">Enter Floor area:</label>
  <input type="text" name="floor-area"> <br>
  <label for="">Select:</label>
  <label for=""><input type="radio" value="rent" name="estab-type" id="estab-rent">Rent</label>
    <label for=""><input type="radio" value="sale" name="estab-type" id="estab-sale">Sale</label>
</fieldset>
</div>
<br>

<div class="estab-rent alfabetBox" >
  <fieldset>
               <label for="rent-value">Rent:</label>
                         <input type="text" name="rent-value1">
               <label for="deposit-value">Deposit:</label>
                         <input type="text" name="deposit-value2"> <br>
              <label for="deposit-value">Enter Turnover:</label>
                         <input type="text" name="deposit-value3">
  </fieldset>
  <br>
 <fieldset>
<label for="">Enter Contact Name:</label>
<input type="text" name="Econtact-name"> <br>
<label for="">Enter Contact Number:</label>
<input type="text" name="Econtact-number">
  </fieldset>
</div>

<div class="estab-sale alfabetBox" >
  <fieldset>
               <label for="rent-value">Enter Selling Cost:</label>
                         <input type="text" name="sale-value1"><br>
               <label for="deposit-value">Enter Turnover:</label>
                         <input type="text" name="sale-value2"> 
             
  </fieldset>
  <br>
 <fieldset>
<label for="">Enter Contact Name:</label>
<input type="text" name="Econtact-name"> <br>
<label for="">Enter Contact Number:</label>
<input type="text" name="Econtact-number">
  </fieldset>
</div>
</div>
 
<div class="right">
     <label style="font-size:30px; padding-left:19px"> Pick Location  </label>
      <br>
    <div class="map" id="poxes">
     <gmap-map
     :center="center"
     :zoom="10"
     style="width:100%;height:400px;" >
     <gmap-marker
      :key="index"
      v-for="(m, index) in markers"
      :position="m.position"
      :title="m.title"
      :clickable="true"
      :draggable="true"
      @click="center=m.position"
>
     </gmap-marker>
     </gmap-map>

   </div>


  <button value="cancel" class="cancel">Cancel</button>  
  <button value="submit" class="submit">Submit</button>


  
</div>
  </form>



  </div>
 </template>
<script>
export default{
  name:'Map',
  data(){
    return{
      center:{lat:12.106527,lng:78.136139},
      currentPlace:null,
      markers:[],
      places:[]
    }
  }

}



  
   
$(document).on('click',"#flat",function(){
    $(".A").show();
    $(".B").hide();
    $(".C").hide();
    $(".plot-sale").hide();
    $(".plot-lease").hide();
     $(".estab-rent").hide();
      $(".estab-sale").hide();
   
     
});
$(document).on('click',"#plot",function(){
    $(".A").hide();
    $(".B").show();
    $(".C").hide();
    $(".rent").hide();
    $(".sale").hide();
     $(".estab-rent").hide();
      $(".estab-sale").hide();
   
});
$(document).on('click',"#estab",function(){
    $(".A").hide();
    $(".B").hide();
    $(".C").show();
    $(".plot-sale").hide();
    $(".plot-lease").hide();
     $(".rent").hide();
    $(".sale").hide();
});
$(document).on('click',"#rent",function(){
    $(".rent").show();
    $(".sale").hide();
   
});


$(document).on('click',"#sale",function(){
    $(".rent").hide();
    $(".sale").show();
   
});

$(document).on('click',"#plot-sale",function(){
    $(".plot-lease").hide();
    $(".plot-sale").show();
   
});

$(document).on('click',"#plot-lease",function(){
    $(".plot-sale").hide();
    $(".plot-lease").show();
   
});

$(document).on('click',"#estab-rent",function(){
    $(".estab-rent").show();
    $(".estab-sale").hide();
   
});

$(document).on('click',"#estab-sale",function(){
    $(".estab-rent").hide();
    $(".estab-sale").show();
   
});





</script>





