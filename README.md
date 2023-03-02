# Mein-taschenrechner
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Taschenrechner</title>

    <link rel="stylesheet" href="manifest.zip">
<!----link css-->
<link rel="stylesheet" href="./stayle.css">

<!---google font-->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Rubik:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap" rel="stylesheet">
<!---java-->
<script>
    function appendOpartion(Opartion) {

document.getElementById('resultArea').innerHTML += Opartion;

    }
    function wert() {

let container = document.getElementById('resultArea');

let result =eval(container.innerHTML);
container.innerHTML = result;
    }

function delet() {

    let container = document.getElementById('resultArea');
container.innerHTML = container.innerHTML.slice(0, -1);
}











</script>

</head>
<body>
    <div id="resultArea"></div>

<table>

    <tr>

        <td></td>
        <td></td>
        <td></td>
        <td onclick="delet()">Del</td>

    </tr>

      


    <tr>

<td onclick="appendOpartion(7)">7</td>
<td onclick="appendOpartion(8)">8</td>
<td onclick="appendOpartion(9)">9</td>
<td onclick="appendOpartion('/')">/</td>



    </tr>


    <tr>

        <td onclick="appendOpartion(4)">4</td>
        <td onclick="appendOpartion(5)">5</td>
        <td onclick="appendOpartion(6)">6</td>
        <td onclick="appendOpartion('*')">x</td>
        
        
            </tr> 
            
            <tr>

                <td onclick="appendOpartion(1)">1</td>
                <td onclick="appendOpartion(2)">2</td>
                <td onclick="appendOpartion(3)">3</td>
                <td onclick="appendOpartion('-')">-</td>
                
                
                
                    </tr>
                    <td onclick="appendOpartion(0)">0</td>
                <td onclick="appendOpartion('.')">,</td>
                <td onclick="wert()" id="re">=</td>
                <td onclick="appendOpartion('+')">+</td>                
                </tr>









</table>




    
</body>
</html>
