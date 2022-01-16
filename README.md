# Web Page for Mathematical Calculations

## AIM:

To design a static website with validation to perform mathematical calculations in client side.

## DESIGN STEPS:

### Step 1:

Requirement collection.

### Step 2:

Creating the layout using HTML and CSS.

### Step 3:

Write javascript to perform the calculations.

### Step 4:

Include regularexpression based input validation.

### Step 5:

Validate the layout in various browsers.

### Step 6:

Validate the HTML code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mathematical Calculations</title>
    <style>
        * {
            box-sizing: border-box;
            font-family: Arial, Helvetica, sans-serif;
        }
        body {
            background-color :rgb(136, 83, 40);
            color: rgb(105, 39, 39);
        }    
       .container {
            width: 700px;
            margin-left: auto;
            margin-right: auto;
            }
        .content {
            display: block;
            width: 100%;
            background-color: cyan;
            min-height: 1000px;
            margin: 0px 0px 0px 0px;
            margin-top: 65px;
            }
        h1{
            text-align: center;
            padding-top: 20px;
            font-style: arial;
        }
        .formelement{
            text-align: center;

        }
        .container2 {
            width: 700px;
            box-sizing: border-box;
            font-family: Arial, Helvetica, sans-serif;
    
            margin-left: auto;
            margin-right: auto;
            }
        .content2 {
            display: block;
            width: 100%;
            background-color: cyan;
            min-height: 500px;
            margin: 0px 0px 0px 0px;
            margin-top: -720px;
            }
        .container3 {
            width: 700px;
            box-sizing: border-box;
            font-family: Arial, Helvetica, sans-serif;
    
            margin-left: auto;
            margin-right: auto;
            }
        .content3 {
            display: block;
            width: 100%;
            background-color: cyan;
            min-height: 500px;
            margin: 0px 0px 0px 0px;
            margin-top: -200px;
            }
            .container4 {
            width: 700px;
            box-sizing: border-box;
            font-family: Arial, Helvetica, sans-serif;

            margin-left: auto;
            margin-right: auto;
            }
        .content4 {
            display: block;
            width: 100%;
            background-color: cyan;
            min-height: 100px;
            margin: 0px 0px 0px 0px;
            margin-top: -230px;
            }
        .footer{
            margin-left: 500px;
            margin-top: 30px;

        
        }  
        
    </style>
</head>
<body>
    <div class="container">
        <div class="content">
            <h1>VOLUME OF A CYLINDER</h1>
            <form>
                <div class="formelement"></br>
                    <label for="aedit">Radius of the cylinder:</label>
                    <input type="text" id="aedit" value="0"/><label for="hedit"> Meters</label>
                </div>
                <div class="formelement">
                </br>
                    <label for="bedit">Height of the cylinder:</label>
                    <input type="text" id="bedit" value="0"/><label for="hedit"> Meters</label>
                </div>
                <div class="formelement">
                </br>
                    <input type="button" value="calculate volume" id="calculate"/>
                </div>
                <div class="formelement">
                </br>
                    <label for="cedit">Volume of the Cylinder:</label>
                    <input type="text" id="cedit" readonly value="0"/><label for="hedit"> Meter<sup>3</sup></label>
                   
                </div>
                
            </form>
            
    </div>
    </div>
<script type="text/javascript">
    var button;
    button=document.querySelector("#calculate");
    button.addEventListener("click",function(){
        var atext,btext,ctext;
        var aval,bval,cval;
        atext=document.querySelector("#aedit");
        btext=document.querySelector("#bedit");
        ctext=document.querySelector("#cedit");
        reg1 = btext.value.match("^[.]?[0-9]+[.]?[0-9]*$");
        reg = atext.value.match("^[.]?[0-9]+[.]?[0-9]*$");
        result = atext.value.match(reg);
        result1= btext.value.match(reg1);
        if(result==null){
            alert("Invalid radius of the cylinder!")
        }else if(result1==null){
            alert("Invalid height of the cylinder!")
        }else{
            ctext.value = 22/7*atext.value*atext.value*btext.value
        }
    });
</script>
     <div class="container2">
        <div class="content2">
            <h1>VOLUME OF A CONE</h1>
            <form>
                <div class="formelement"></br>
                    <label for="dedit">Radius of the Cone:</label>
                    <input type="text" id="dedit" value="0"/><label for="hedit"> Meters</label>
                </div>
                <div class="formelement">
                </br>
                    <label for="fedit">Height of the cone:</label>
                    <input type="text" id="fedit" value="0"/><label for="hedit"> Meters</label>
                </div>
                <div class="formelement">
                </br>
                    <input type="button" value="calculate volume" id="solve"/>
                </div>
                <div class="formelement">
                </br>
                    <label for="gedit">Volume of the Cone:</label>
                    <input type="text" id="gedit" readonly value="0"/><label for="gedit"> Meter<sup>3</sup></label>
                </div>
            </form>
    </div>
    </div>
<script type="text/javascript">
    var button;
    button=document.querySelector("#solve");
    button.addEventListener("click",function(){
        var dtext,ftext,gtext;
        var dval,fval,gval;
        dtext=document.querySelector("#dedit");
        ftext=document.querySelector("#fedit");
        gtext=document.querySelector("#gedit");
        reg3 = dtext.value.match("^[.]?[0-9]+[.]?[0-9]*$");
        reg4 = ftext.value.match("^[.]?[0-9]+[.]?[0-9]*$");
        result3 = dtext.value.match(reg3);
        result4= ftext.value.match(reg4);
        if(result3 == null){
            alert("Invalid radius of the cone!")
        }else if(result4 == null){
            alert("Invalid height of the cone")
        }else{
            gtext.value = 22/7*dtext.value*dtext.value*ftext.value/3;

        }

    });
</script>
<div class="container3">
    <div class="content3"> 
        <h1>AREA OF A RECTANGLE</h1>
        <form>
            <div class="formelement"></br>
                <label for="xedit">Length of a rectangle:</label>
                <input type="text" id="xedit" value="0"/><label for="hedit"> Meters</label>
            </div>
            <div class="formelement">
            </br>
                <label for="yedit">Breadth of a rectangle:</label>
                <input type="text" id="yedit" value="0"/><label for="hedit"> Meters</label>
            </div>
            <div class="formelement">
            </br>
                <input type="button" value="calculate area" id="calculatearea"/>
            </div>
            <div class="formelement">
            </br>
                <label for="zedit">Area of the rectangle:</label>
                <input type="text" id="zedit" readonly value="0"/><label for="hedit"> Meter<sup>2</sup></label>
            </div>
        </form>
</div>
</div>
<script type="text/javascript">
var button;
button=document.querySelector("#calculatearea");
button.addEventListener("click",function(){
    var xtext,ytext,ztext;
    var xval,yval,zval;
    xtext=document.querySelector("#xedit");
    ytext=document.querySelector("#yedit");
    ztext=document.querySelector("#zedit");
    xreg = xtext.value.match("^[.]?[0-9]+[.]?[0-9]*$")
    yreg = ytext.value.match("^[.]?[0-9]+[.]?[0-9]*$")
    xresult = xtext.value.match(xreg)
    yresult = ytext.value.match(yreg)
    if(xresult == null){
        alert("Invalid Length of Rectangle")
    }else if(yresult == null){
        alert("Invalid Height of Rectangle")
    }else{
        ztext.value = xtext.value*ytext.value
    }
});
</script>
</script>
<div class="container4">
    <div class="content4">
        <h1>VOLUME OF A RECTANGULAR PRISM</h1>
        <form>
            <div class="formelement"></br>
                <label for="ledit">Length:</label>
                <input type="text" id="ledit" value="0"/><label for="nedit"> Meters</label>
            </div>
            <div class="formelement">
            </br>
                <label for="medit">Width:</label>
                <input type="text" id="medit" value="0"/><label for="nedit"> Meters</label>
            </div>
            <div class="formelement">
            </br>
                <label for="oedit">height:</label>
                <input type="text" id="oedit" value="0"/><label for="nedit"> Meters</label>
            </div>
            <div class="formelement">
            </br>
                <input type="button" value=" calculate volume" id="volumebutton"/>
            </div>
            <div class="formelement">
            </br>
                <label for="sedit">volume of a rectangular prism:</label>
                <input type="text" id="sedit" readonly value="0"/><label for="nedit"> Meter<sup>3</sup></label>
        </div>
        
        </form>
        <div class="footer">D.Vishnu vardhan reddy.</div>
</div>
</div>
<script type="text/javascript">
var button;
button=document.querySelector("#volumebutton");
button.addEventListener("click",function(){
    var ltext,mtext,oedit,stext;
    var lval,mval,oedit,sval;
    ltext=document.querySelector("#ledit");
    mtext=document.querySelector("#medit");
    otext=document.querySelector("#oedit");
    stext=document.querySelector("#sedit");
    regl = ltext.value.match("^[.]?[0-9]+[.]?[0-9]*$")
    regm = mtext.value.match("^[.]?[0-9]+[.]?[0-9]*$")
    rego = otext.value.match("^[.]?[0-9]+[.]?[0-9]*$")
    resultl = ltext.value.match(regl)
    resultm = mtext.value.match(regm)
    resulto = otext.value.match(rego)
    if(resultl == null){
        alert("Invalid Length of Rectangular Prism")
    }else if(resultm ==null){
        alert("invalid width of Rectangular Prism")
    }else if(resulto == null){
        alert("Invalid height of Rectangual Prism")
    }else{
        lval = parseInt(ltext.value);
    mval = parseInt(mtext.value);
    oval = parseInt(otext.value);
    sval = lval*mval*oval;
    stext.value=""+sval;
    }

});
</script>
</body>
</html>

```

## OUTPUT:

![OUTPUT](/IMAGES/web.png)

## Result:

Thus a website is designed to perform mathematical calculations in the client side.
