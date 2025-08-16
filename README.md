<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Learning HTML</title>

    <style>

        body{
            background-color: #af1212d2;
        }

        .painel{
            margin:auto;
            width: 500px;
            height: 500px;
            border-radius: 20px;
            text-align: center;
            padding-top: 50px;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;

        }
        #sim{
            
            
            height: 40px;
            width: 60px;
            background-color: rgb(247, 245, 245);
            border: 2px solid black;
            border-radius: 10px;
            color:black;
            margin-left: -50px;
        }
        #nao
        {
            position: absolute;
            height: 40px;
            width: 60px;
            background-color: rgb(255, 255, 255);
            border: 2px solid black;
            border-radius: 10px;
            color:black;
            margin-left: 20px;
        }
    </style>

</head>
<body>
    
    <div class="painel">
        <h1>Quer sair comigo hoje?</h1> 

        

        <a href="http://127.0.0.1:5500/working.html"><button id="sim"> Sim!</button>
        <button onmouseover="fuja()" id="nao"> Não!</button>

        
       
        
    </div>

    <script>
        function fuja(){
            var botaoNao = document.getElementById("nao")

            var larguraJanela = window.innerWidth;
            var alturaJanela = window.innerHeight;

            var maxX = larguraJanela - botaoNao.offsetWidth;
            var maxY = alturaJanela - botaoNao.offsetHeight;

            var aleatorioX = Math.floor(Math.random() * maxX);
            var aleatorioY = Math.floor(Math.random() * maxY);

            botaoNao.style.left = aleatorioX + "px";
            botaoNao.style.top = aleatorioY + "px";
        }
    </script>

    

</body>
</html>
