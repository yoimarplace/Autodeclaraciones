# Flujo-de-autodeclaracion

1.	Para generar la declaración se debe consumir el metodo **income-request-aio**, enviando la trama de información de la empresa y el declarante junto con la URL de retorno en el objeto: returnURL.

2.  Placetopay responde con el identificador: requestID y el redirecTO.

3.	Guardar el requestID en relación al usuario.

4.  Redirecciona al usuario al redirecTO obtenido en el punto 2.

5.	En la interfaz se visualiza el formato PDF con la información suministrada, para proceder con las firmas virtuales.

6.	El representante legal y ( el revisor fiscal ) autorizan para que la declaración pueda ser pagada.

7.	El declarante puede proceder con el pago, el cual es redireccionado a la interfaz de pagos Placetopay para realizar el proceso transaccional.

8.	Al finalizar el pago, el sistema añade al PDF el cello que certifica que la declaración ha sido paga.

9.  Una vez el usuario da clic en “Regresar al comercio”, éste es enviado a la URL de retorno returnUrl (Atributo especificado al crear la operación).

10.  Para consultar el estado de la declaración se debe consumir el metodo information-request enviando el requestID

11. Para descargar el pdf se debe consumir el metodo income-pdf enviando el requestID y el locale.


[Imagen de flujo](https://lucid.app/publicSegments/view/890a7af8-73bd-49f1-a91d-511cca52a1b4/image.pdf)

