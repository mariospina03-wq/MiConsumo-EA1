# MiConsumo - EA1

Proyecto de Programacion Orientada a Objetos en C++ para estimar el consumo
semanal y mensual de equipos del hogar mediante las clases `Equipo` y `Hogar`,
vectores, un vector de objetos y una matriz.

## Contenido

- `miconsumo.cpp`: programa y menu interactivo.
- `Román_Maribel_EA1 Programa orientado a objetos con vectores y matrices.pdf`:
  informe de la evidencia.
- `capturas_ea1/`: pruebas capturadas desde la terminal y recorte de la factura.

## Compilar y ejecutar

Con g++ instalado (por ejemplo, MSYS2 UCRT64):

```bash
g++ -std=c++11 -Wall -Wextra -pedantic miconsumo.cpp -o miconsumo
./miconsumo
```

En el menu, la opcion 6 carga los cuatro equipos; las opciones 4 y 5 muestran
la matriz y el reporte, la opcion 7 simula un ahorro y la opcion 8 consulta
un equipo.

## Datos y supuestos

Los datos del informe y la factura corresponden al material suministrado por la
estudiante. El perfil distribuye las tres lavadas en martes, jueves y sabado, y
los usos de la freidora en lunes, miercoles y viernes: los dias no fueron
especificados y esta distribucion es un supuesto que se puede editar.

Las etiquetas de refrigerador y congelador reportan kWh/mes, no potencia en W;
el programa calcula potencias promedio equivalentes para estimar la semana. La
lavadora tambien usa una potencia equivalente inferida con el supuesto de una
hora por ciclo. Los resultados son estimaciones, no mediciones directas.

La simulacion reduce matematicamente el uso del equipo y no debe interpretarse
como una recomendacion para desconectar equipos de refrigeracion.
