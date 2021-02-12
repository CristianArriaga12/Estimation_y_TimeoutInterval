# Estimation_y_TimeoutInterval
## Práctica 2 
## Redes de Computadoras

### Estimación del temporizador de retransmisión (RTO, retransmission timeout) en TCP

En este repositorio encontraremos scripts y archivos generados durante el proceso de estimación del proceso de RTT, con el fin de predecir el tiempo de espera del emisor, con el fin de ver los tiempos de retransmisión.

### Desarrollo

Se descargaron 4 Trazas proporcionadas por el Dr Reni Torres del CINVESTAV y posteriormente proporcionados por el Dr. Victor Ramos de la UAM-I, para el estudio del tiempo de retransmisión para la práctica 2 del curso de Redes de telecomunicaciones.

Posteriormente se utilizaron dichas tramas para calcular 
EstimatedRTTi = (1-α)*EsimatedRTTi-1 + α*SampleRTTi
Donde SampleRTT es la muestra original que obtenemos desde la trama descargada

Posteriormente la guardaremos en un nuevo archivo de texto llamado EstimatedRTT.txt

Cabe señalar que en el primer dato, debemos tomar en cuenta que no tenemos un EstimatedRTT(0-1), por tanto elegiremos que el primer dato será EstimatedRTT= SampleRTT y con los valores estándar α=0.125 & β=0.25

Como segundo paso calcularemos la Desviación,
