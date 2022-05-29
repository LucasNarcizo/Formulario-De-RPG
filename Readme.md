<!DOCTYPE html>
<HTML lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulario | GN</title>
    <style>
        body{
            font-family: Arial, Helvetica, sans-serif;
            background-image: linear-gradient(to right, rgba(110, 1, 219, 0.658), rgba(189, 0, 241, 0.733));
        }
        .box{
            color: white;
            position: absolute;
            top:25%;
            left:35%;
            transform: translate(-10%, -10%);
            background-color: rgba(0, 0, 0, 0.5);
            padding: 15px;
            border-radius: 15px;
            width: 25%;
             
        }
        fieldset{
            border: 3px solid darkviolet;
        }
        legend{
            border: 1px solid darkorchid;
            padding: 5px;
            text-align: center;
            background-color: darkviolet;
            border-radius: 5px;
        }
        .inputbox{
            position: relative;
        }
        .inputUser{
            background: none;
            border: none;
            border-bottom: 1px solid white;
            color: white;
            font-size: 15px;
        }
        .labelInput{
            position: absolute;
            top:0px;
            left:0px;
            pointer-events: none;
            transition: 3s;
        }
       
        .inputUser:focus ~ .labelInput,
        .inputUser:valid ~ .labelInput{
            
            top:-20px;
            font-size: 12px;
            color: rgb(189, 146, 230);
        }
        #data_nascimento{
            border: none;
            padding: 6px;
            border-radius: 10px;
        }
        #submit{
            background-image: linear-gradient(to right, rgba(118, 13, 204, 0.658), rgba(200, 12, 247, 0.733));
            width: 100%;
            border:none;
            border-radius: 10px;
            padding: 10px;
            color: white;
            cursor: pointer;


        }
        #submit:hover{
            background-image: linear-gradient(to right, rgba(28, 4, 48, 0.658), rgba(73, 33, 83, 0.733));
        }

    </style>
</head>
<body>
    <div class="box">
        <form action="">
            <fieldset>
                <legend><b>Formulario de RPG</b></legend>
                <div class="inputbox">
                    <input type="text" name="" id="nome" class="inputUser" required>
                    <label for="nome" class="labelInput">Nome Completo</label>
                </div>
                <br><br>
                <div class="inputbox">
                    <input type="text" name="email" id="email" class="inputUser" required>
                    <label for="email" class="labelInput">Email</label>
                </div>
                <br><br>
                <div class="inputbox">
                    <input type="text" name="Funcao" id="Funcao" class="inputUser" required>
                    <label for="Funcao" class="labelInput">Função</label>
                </div>
                <div class="inputbox">
                    <p>Genero:</p>
                    <input type="radio" id="masculino" name="genero" value="masculino" required>
                    <label for="masculino">Masculino</label>
                    <br>
                    <input type="radio" id="feminino" name="genero" value="feminino" required>
                    <label for="feminino">Feminino</label>
                    <br>
                    <input type="radio" id="outro" name="genero" value="outro" required>
                    <label for="outro">Outros   </label></div>
            <br>
            <div class="inputbox">
                <label for="data_nascimento"><b>Data de Nascimento</b></label>
                <input type="date" name="data_nascimento" id="data_nascimento" required>
            <br><br>
            <div class="inputbox">  
                <input type="text" name="classe" id="classe" class="inputUser" required>
                <label for="classe" class="labelInput">Classe</label>
            </div>
            <br><br>
            <div class="inputbox">
                <input type="text" name="raca" id="raca" class="inputUser" required>
                <label for="raca" class="labelInput">Raça</label>
            </div>
            <br><br>
            <div class="inputbox">   
                <input type="text" name="level" id="level" class="inputUser" required>
                <label for="level" class="labelInput">Level</label>
            </div>
             <br><br>
            <input type="submit" name="submit" id="submit">
        <form>
    </div>
</body>
</HTML> 

