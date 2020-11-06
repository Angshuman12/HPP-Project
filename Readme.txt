<!DOCTYPE html>
<html >
<head>
  <meta charset="UTF-8">
  <title>Assam house price prediction</title>
 
  <style>
   
      body {
      background-image: url('ak4.jpg');    
      background-repeat: no-repeat;
      background-attachment: fixed;
      background-size: cover;
    }
 
    h1   {color: yellow;}  /* CSS code for heading h1 */
    p   {color: yellow;}  /* CSS code for heading h1 */
 
    /* CSS code for button */
    .button_css {
    color: Red;
    text-transform: uppercase;
    text-decoration: none;
    background: #ffffff;
    padding: 20px;
    border: 4px solid #494949 !important;
    display: inline-block;
    transition: all 0.4s ease 0s;
    }
     
    .button_css:hover {
    color: #ffffff !important;
    background: #f6b93b;
    border-color: #f6b93b !important;
    transition: all 0.4s ease 0s;
    }
     
    .footer {
  position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
  background-color: red;
  color: yellow;
  text-align: center;
   
  /* unvisited link */ 
  a:link { color: White; } 
  /* visited link */ 
  a:visited { color: green; }
}   
  </style>
 
</head>
 
<body>
 
  
 
  
  
 <div class="login">
     
    <!-- Form Get input to predict Marks-->
    <center>
    <form action="{{ url_for('predict')}}"method="post">
        <h1>*Enter the Information of House to Predict the Price*</h1>
         
        <input align="center" type="number" name="bathrooms" placeholder="Bathrooms" required="required" width="48" height="10" step=".01"/><br>
        <input align="center" type="number" name="balcony" placeholder="Balcony" required="required" width="48" height="10" step=".01"/><br>
        <input align="center" type="number" name="total_sqft_int" placeholder="Total Squre Foot" required="required" width="48" height="10" step=".01"/><br>
        <input align="center" type="number" name="bhk" placeholder="BHK" required="required" width="48" height="10" step=".01"/><br>
        <input type="text" name="location" placeholder="House Location" required="required" />  <br> 
        <input type="text" name="location" placeholder="Property Type" required="required" /> <br>
<input align="center" type="number" name="age" placeholder="Property Age" required="required" width="48" height="10" step=".01"/><br>
        


    
 
        <br>
         
        <br>
         
        <!-- Show button -->
        <div class="button_cont" align="center"><a class="button_css" href=/" target="_blank" rel="nofollow noopener">
            <button type="submit" class="btn btn-primary btn-block btn-large"><strong>Predict House Price</strong></button></a>
        </div>
         
    </form>
    </center>
    
   <!-- Show predicted output using ML model --> 
   
 
 </div>
 
 <div class="footer">
 </div>
</body>
</html>