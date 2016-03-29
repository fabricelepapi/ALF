# ALF
Le devoir consistait à ecrire un programme PEG.js pour valider si un numero de carte de credit est vadid ou non
voici mon code dans un fichier PEG.js
function cardnumber(inputtxt)  
{  
  var cardno = /^(?:4[0-9]{12}(?:[0-9]{3})?)$/;  
  if(inputtxt.value.match(cardno))  
        {  
      return true;  
        }  
      else  
        {  
        alert("Not a valid Visa credit card number!");  
        return false;  
        }  
        
}
Dans  html
<html>  
<head>  
<meta charset="utf-8">  
<title>exo2</title>         
</head>
<br>
<body onload='document.form1.text1.focus()'>  
<h2>FABRICE -Credit card checker-</h2>  
<form name="form1" action="#">  
<input type='text' name='text1'/>  
<input type="submit" name="submit" value="Submit" onclick="cardnumber(document.form1.text1)"/> 
</form>  
<script src="PEG.js"></script>  
</body>  
</html> 
pour tester 
Si on utilise xmap  : go to this directory : c://xmap/htdoc/ 

creer un dossier : ex : fabrice 

copier les deux dossier : index.html & PEG.js 

aller sur le browser , ecrire ceci : localhost/[name_of_folder] which is : localhost/fabrice 
