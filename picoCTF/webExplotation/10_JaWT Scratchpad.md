# Level X
## Objetivo
> Check the admin scratchpad! `https://2019shell1.picoctf.com/problem/32267/` or [http://2019shell1.picoctf.com:32267](http://2019shell1.picoctf.com:32267/)
## Pistas
What is that cookie? Have you heard of JWT?
## Solucion
Cuando ingresamos a este enlace, nos recibe una aplicación web de bloc de notas de algún tipo. Nos permite acceder a cualquier usuario además de "admin". Cuando nos deja pasar, vemos una cookie emergente en la pestaña Aplicación de las herramientas para desarrolladores de Chrome llamada "jwt". Esto almacena una larga secuencia de caracteres. Si buscamos "jwt", descubrimos que es un token web JSON que consta de tres componentes: el encabezado, la carga útil y la firma. Si decodificamos la cookie jwt que obtuvimos en jwt.io, vemos en el encabezado que se trata de un jwt que utiliza el algoritmo HS256. La carga útil es solo un valor: nuestro nombre de usuario. Sabemos que el nombre de usuario correcto es "admin", ya que es a quien el sitio web no permite iniciar sesión, pero no conocemos la firma. A partir de aquí, necesitamos usar JohnTheRipper, que está vinculado en el sitio de JaWT Scratchpad bajo la entrada de nombre. JohnTheRipper utiliza un método de fuerza bruta para averiguar la firma de jwt. Sin embargo, es muy lento, ya que tiene que pasar por tantas posibilidades. Una mejor manera es usar una lista de palabras. Lo que es una lista de palabras es un diccionario de secretos comunes para JohnTheRipper para reducir las posibilidades y descifrar la firma más rápido. Esto podría significar la diferencia entre varias horas y unos pocos segundos. Una lista de palabras muy fuerte es rockyou, que tiene una colección masiva de palabras comunes. Después de ejecutar esto, JohnTheRipper te da el secreto: ilovepico. Puede volver a jwt.io y ponerlo junto con el usuario en la carga útil como 'admin'. Inserte esto como su cookie jwt e inicie sesión para evitar el portal y obtener la bandera
## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias
