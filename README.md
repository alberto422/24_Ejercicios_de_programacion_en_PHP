24_Ejercicios_de_programacion_en_PHP
====================================


Primer Ejercicio de 24 
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
        
        
        
        
        
        
   
<!--Segundo Ejercicio de 24-->

            <!--Arias Mero Alberto Fernando
                Tercer Nivel "A"-->
            
 <title>Segundo Ejercicio</title>
 <h1 >Segundo Ejercicio</h1>
 
        <?php
       ini_set('display_errors', 'off');
       ini_set('display_startup_errors', 'off');
       error_reporting(0);
       
       function segundo_ejercicio()
       {
           
       $valorx= $_POST['ingresox'];
       $valory= $_POST['ingresoy'];
       
       if ($_POST['enviar']) 
        {
            $valores_en_x = [2, 2, 4, 12, 48];
            $valores_en_y = [3, 3, 6, 18, 72];
            if ($valorx==0 or $valory==0 or $valorx<0 or $valory<0 or $valorx>255 or  $valory>255){
                echo ''-1;
                return FALSE;
               }
                if ($valorx==2) {
                  $mostrar = $valores_en_x[$valory];
                  echo 'El valor es : '.$mostrar;
               }
             else  if ($valorx==3) {
                  $mostrar = $valores_en_y[$valory];
                  echo 'El valor es : '.$mostrar;
                   
               }
        }else
           {
        ?>
        <form method="post" action="Segundo_ejercicio.php">
            <div>Ingresa X :<input type="text" name="ingresox" maxlength="3"></div>
            <div>Ingresa Y :<input type="text" name="ingresoy" maxlength="3"></div>
            <input type="submit" name="enviar" value="Verificar ">
         </form>
 
        <?php 
          }
        
       } return segundo_ejercicio();
        ?>

   
   
   
   
   
   
<!--Tercer Ejercicio de 24-->

            <!--Arias Mero Alberto Fernando
                Tercer Nivel "A"-->
            
 <title>Tercer Ejercicio</title>
 <h1 >Tercer Ejercicio</h1>
        
     <?php
     ini_set('display_errors', 'off');
     ini_set('display_startup_errors', 'off');
     error_reporting(0); 
     
     function Tercer_ejercicio(){
          $valorx= $_POST['ingresox'];
          $valory= $_POST['ingresoy'];
          
     if ($_POST['enviar']) 
     {
        $valores = ["",60, 30, 20, 15, 12];
        
        if ($valorx==0 or $valory==0 or $valorx<0 or $valory<0 or $valorx>255 or $valory>255) {
            echo ''-1;
        }
        else if ($valorx== $valores[1]) {
            $resultado = $valores[$valory];
             echo ''.$resultado;
        }
        
         
     }else
         {
     ?>
        <form method="post" action="Tercer_ejercicio.php">
            <div>Ingresa X :<input type="text" name="ingresox" maxlength="3"></div>
            <div>Ingresa Y :<input type="text" name="ingresoy" maxlength="3"></div>
            <input type="submit" name="enviar" value="Verificar ">
         </form>
 
    <?php
         }
     }     return Tercer_ejercicio();
    ?>
