# temperature
temperature convertor
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="widt
initial-scale=1.0">
    <title>Temperature convertor</title
    <style>
        body{
            padding: 50px 100px;

        }
        h1{
            text-align: center;
        }
        #container{
            text-align: center;
            background-color: aqua;
            padding: 50px;
        }
        .input-div{
            display: inline-block;
        }
        .inp{
            padding: 5px 10px;
            margin:10px;
            font-size: 30px;
            font-weight: bold;
            width:250px;
            text-align:center;
        }
        label{
            font-size:22px;
            color: black;
        }
    </style>
</head>
<body>
    <h1>Temperature convertor</h1>
    <div id="container">
        <div class="input-div">
            <label >celcius</label><br>
            <input type="number" value=
id="cel"class="inp">
        </div>
        <div class="input-div">
            <label >fahrenheit</label><
            <input type="number" value=
id="fah"class="inp">
        </div>
    </div>
    <script>
        var cel=document.getElementById
        var fah=document.getElementById
        cel.addEventListener('input', f
            let c=this.value;
            let f=(c * 9/5) + 32;
            
            

            
            fah.value=f; 
        
            

        });
        fah.addEventListener('input',
function(){
    let f=this.value;
    let c= (f -32) * 5/9;
    
    
 
    cel.value=c; 

 });
 
    </script>
</body>
</html>
