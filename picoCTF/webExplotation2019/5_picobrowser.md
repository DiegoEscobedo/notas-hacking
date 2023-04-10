## Descripción
This website can be rendered only by picobrowser, go and catch the flag! 

## Pistas 
You don't need to download a new web browser

## Solución
Lo que tenemos que hacer es cambiar el valor del User-Agent en las herramientas del desarrollador para que piense que lo estamos haciendo desde "picobrowser" y no desde nuestro navegador usual.
Actualizamos la página y tenemos la bandera.
O desde terminal 
C:\Users\diego>curl -s https://jupiter.challenges.picoctf.org/problem/50522/flag -H "User-Agent: picobrowser" | grep picoCTF
"grep" no se reconoce como un comando interno o externo,
programa o archivo por lotes ejecutable.

C:\Users\diego>curl -s https://jupiter.challenges.picoctf.org/problem/50522/flag -H "User-Agent: picobrowser"
<!DOCTYPE html>
<html lang="en">

<head>
    <title>My New Website</title>


    <link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap.min.css" rel="stylesheet">

    <link href="https://getbootstrap.com/docs/3.3/examples/jumbotron-narrow/jumbotron-narrow.css" rel="stylesheet">

    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>

    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>

</head>

<body>

    <div class="container">
        <div class="header">
            <nav>
                <ul class="nav nav-pills pull-right">
                    <li role="presentation" class="active"><a href="/">Home</a>
                    </li>
                    <li role="presentation"><a href="/unimplemented">Sign In</a>
                    </li>
                    <li role="presentation"><a href="/unimplemented">Sign Out</a>
                    </li>
                </ul>
            </nav>
            <h3 class="text-muted">My New Website</h3>
        </div>

       <!-- Categories: success (green), info (blue), warning (yellow), danger (red) -->


       <div class="alert alert-success alert-dismissible" role="alert" id="myAlert">
         <button type="button" class="close" data-dismiss="alert" aria-label="Close"><span aria-hidden="true">&times;</span></button>
         <!-- <strong>Title</strong> --> picobrowser!
           </div>



        <div class="jumbotron">
            <p class="lead"></p>
            <p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{p1c0_s3cr3t_ag3nt_51414fa7}</code></p>
            <!-- <p><a class="btn btn-lg btn-success" href="admin" role="button">Click here for the flag!</a> -->
            <!-- </p> -->
        </div>


        <footer class="footer">
            <p>&copy; PicoCTF 2019</p>
        </footer>

    </div>
    <script>
    $(document).ready(function(){
        $(".close").click(function(){
            $("myAlert").alert("close");
        });
    });
    </script>
</body>

</html>
C:\Users\diego>
## Bandera
picoCTF{p1c0_s3cr3t_ag3nt_51414fa7}

## Notas Adicionales

## Referencias
https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/User-Agent