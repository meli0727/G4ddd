<!DOCTYPE html>
<html xmlns=""> 
  <head>  
    <title>Meli's Menu</title>   
    <link rel="stylesheet" href="Form.css"> 
  </head>
    <body> 
    <form name="Menu">     
    <fieldset>
        <legend>Menu</legend>         
        <div>          
          <p>Pick A Pizza</p>             
          <p><input type="radio" value="Cheese Pizza" name="WW" /> Cheese Pizza</p>             
          <p><input type="radio" value="Three Meat Pizza" name="WW" /> Three Meat Pizza</p>             
          <p><input type="radio" value="Sausage Pizza" name="WW" />Sausage Pizza</p>             
          <p><input type="radio" value="Veggie Pizza" name="WW" /> Veggie Pizza</p>         
        </div>                 
          <br />            
        <div>             
          <p>Pick A Salad</p>             
          <p><input type="checkbox" value="Caesar Salad" name="SS" /> Caesar Salad</p>             
          <p><input type="checkbox" value="Chicken Salad" name="SS" /> Chicken Salad</p>             
          <p><input type="checkbox" value="Egg Salad" name="SS" /> Egg Salad</p>             
          <p><input type="checkbox" value="Garden Salad" name="SS" /> Garden Salad</p>           
        </div>       
     </fieldset>      
    <fieldset>         
        <legend>Pick Two Sides</legend>            
        <div>             
          <p>Fruit</p>                
          <select name="FF">                
              <option value="Pineapple">Pineapple</option>                   
              <option value="Grapes">Grapes</option>                   
              <option value"Apple">Apple</option>              
          </select>             
          <br />                 
          <p>Fries</p>            
            <input type="button" value="Plain Fries" onclick="answerP()"/>            
            <input type="button" value="Curly Fries" onclick="answerC()"/>            
            <input type="button" value="Cheese Fries" onclick="answerE()"/>             
          <br />            
        </div>         
      </fieldset>        
      <fieldset>           
        <div>        
         <p>Anything We Should Know About Your Order</p>         
         <p><input name="RR" type="text" placesholder="Anything Extra" /></p>            
         <p>What is your favourite color? <input name="PP" type="color"/>(The color that you choose is going to be your pizza box color)</p>      
        </div>         
        <div>         
        <p>Thanks For Ordering!</p>            
        <input type="submit" onclick="answerChecker()"/>           
        </div>           
        <div>         
          <p>Thanks For Ordering!</p>           
        </div>        
      </fieldset>    
  </form>    
  <script> 
    function answerChecker() {  
          //check which option is choosen on select menu  
          if(document.Menu.WW.value==="Cheese Pizza") {   
          alert("This is our Special Pizza!");  } 
          else {   alert("WE ARE OUT OF THAT PIZZA,SORRY!");  
      }  
          //check which option is choosen on select menu  
          if(document.Menu.SS.value==="Garden Salad"){   
          alert("You have to pay 50 more cents for Garden Salad");  } 
          else {   alert("WE ARE OUT OF SALAD,SORRY");  
       }  
          //check which option is choosen on select menu  
          if(document.Menu.FF.value==="Pineapple") {   
          alert("You have to pay 50 more cents for Pineapple");  } 
          else {   alert("WE ARE OUT OF THAT KIND OF FRUIT,SORRY");  
      }  
          //check which option is choosen on select menu   
          if(document.Menu.RR.value==="More Cheese!!!") {   
          alert("That's Great to know!!");  } 
          else {   alert("Thanks for telling us!!!");  
      }  
          //check which option is choosen on select menu   
          if(document.Menu.PP.value==="#FFF") {   
          alert("I like that color too!!");  } 
          else {   alert("That's a great color for a pizza box!");  
      }  
      }  
      function answerP(){  alert("Plain Fries are the best!!!"); 
  }  
      function answerC(){  alert("Curly Fries are awesome!!!"); 
  }  
      function answerE(){  alert("Cheese Fries are great!!!"); 
  } 
  </script>
</body>
</html>
