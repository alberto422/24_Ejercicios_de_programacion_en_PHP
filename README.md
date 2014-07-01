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






<!--Cuarto Ejercicio de 24-->

            <!--Arias Mero Alberto Fernando
                Tercer Nivel "A"-->
        
 <title>Cuarto Ejercicio</title>
 <h1 >Cuarto Ejercicio</h1>
 
   <?php
     ini_set('display_errors', 'off');
     ini_set('display_startup_errors', 'off');
     error_reporting(0); 
     
     function Cuarto_ejercicio(){
         
         $cadena1= $_POST['S1'];
         $cadena2= $_POST['S2'];
         
     if ($_POST['enviar']) {
        
         if(strcmp($cadena1,$cadena2) == 0)
{
echo "El string ".$cadena1." y string ".$cadena2." Son iguales";
}else
  {
echo "El string ".$cadena1." y string ".$cadena2." no Son iguales <br />";

for ($i = 0; $i < strlen($cadena1.$cadena2); $i++) 
    {
    while ($cadena1[$i] != $cadena2[$i]) 
        {
        $valor= $cadena1[$i];
        print  ($valor) ;  return TRUE;                       
        }
    }
  }  
     }else
         {
        ?>
        <form method="post" action="Cuarto_ejercicio.php">
            Ingresa Primer Texto :<div><input type="text" name="S1" maxlength="60"></div>
            Ingresa Segundo Texto :<div><input type="text" name="S2" maxlength="60"></div>
            <input type="submit" name="enviar" value="Verificar ">
         </form>
 
     <?php 
        }
     }return Cuarto_ejercicio();
     
     ?>

  

  


<!--Sexto Ejercicio de 24-->

            <!--Arias Mero Alberto Fernando
                Tercer Nivel "A"-->
            
   <title>Sexto Ejercicio</title>
   <h1 >Sexto Ejercicio</h1>

   <?php

     ini_set('display_errors', 'off');
     ini_set('display_startup_errors', 'off');
     error_reporting(0); 
     
       function Sexto_ejercicio()
     {
         
         $frase= $_POST['frase'];
                 
     if ($_POST['enviar']) 
     {
         foreach(array_reverse(explode(" ", $frase)) as $frase)
         {
             echo $frase." ";
         }
      
     }else
         {
        ?>
        <form method="post" action="Sexto_ejercicio.php">
            Ingrese Una Frase :<div><input type="text" name="frase" ></div>
            <input type="submit" name="enviar" value="Verificar ">
         </form>
 
     <?php 
     
        }
     }return Sexto_ejercicio();
     
     ?>





<!--Noveno Ejercicio de 24-->

            <!--Arias Mero Alberto Fernando
                Tercer Nivel "A"-->
            
 <title>Noveno Ejercicio</title>
 <h1 >Noveno Ejercicio</h1>
  
     <?php
     ini_set('display_errors', 'off');
     ini_set('display_startup_errors', 'off');
     error_reporting(0); 
     
       function Noveno_ejercicio(){
         
         $valor= $_POST['valor'];
                 
     if ($_POST['enviar']) {
       
         
         for ($recoree = 1; $recoree <= $valor; $recoree++) 
         {
             $potencia = $recoree * $recoree;
             
             while ($valor == $potencia) 
                 { $Bandera= 1;  echo  "TRUE";   return TRUE;}                  
         }  echo 'FALSE';
         
          if ($Bandera > 0) 
              { echo 'FALSE'; }
        
         
     }else
         {
        ?>
        <form method="post" action="Noveno_ejercicio.php">
            Ingrese Numero Positivo :<div><input type="text" name="valor" ></div>
            <input type="submit" name="enviar" value="Verificar ">
         </form>
 
     <?php 
     
        }
     }return Noveno_ejercicio();
     
     ?>

  



