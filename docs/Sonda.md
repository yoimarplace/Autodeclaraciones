# Sonda

El sistema de **sonda** es una tarea programada o **Cron job** que se ejecuta cada cierto periodo de tiempo. En este caso Cada 5 minutos en prueba y cada 24 horas en producción.


Esta programación se debe llevar a cabo por el ente territorial para la actualización de las transacciones que queden en estado **"PENDIENTE"**. en caso de la que declaración no requiera pago (valor de pago = 0) no se debe realizar proceso de sonda, el estado de la declaración será "Presentado".

