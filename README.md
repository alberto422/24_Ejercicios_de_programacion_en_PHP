24_Ejercicios_de_programacion_en_PHP
====================================

<!--Primer Ejercicio de 24-->

            <!--Arias Mero Alberto Fernando
                Tercer Nivel "A"-->
     <title>Primer Ejercicio</title>
     <h1 >Primer Ejercicio</h1>

        <?php
         ini_set('display_errors', 'off');
         ini_set('display_startup_errors', 'off');
         error_reporting(0);
         
        function Primer_Ejercicio(){
            
        $valorx= $_POST['ingresox'];
        $valory= $_POST['ingresoy'];
        
        if ($_POST['enviar']) 
          {
            $valores = ["",7, 6, 8, 4, 9, 2, 10, 0, 11, -2];
            if ($valorx==0 or $valory==0 or $valorx<0 or $valory<0 or $valorx>255 or  $valory>255){
                echo ''-1;
              
            }
           else if ($valores[$valorx] and $valores[$valory]){
                $suma= $valores[$valorx]+$valores[$valory];
                echo 'la suma es : '.$suma;    
            }        
          }else {
       ?>
        <form method="post" action="Primer_ejercicio.php">
            <div>Ingresa X :<input type="text" name="ingresox" maxlength="3"></div>
            <div>Ingresa Y :<input type="text" name="ingresoy" maxlength="3"></div>
            <input type="submit" name="enviar" value="Verificar o Sumar">
         </form>
        
        <?php
               }
        
        } return Primer_Ejercicio();
        ?>
        
