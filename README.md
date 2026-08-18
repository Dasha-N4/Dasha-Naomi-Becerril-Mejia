# Dasha-Naomi-Becerril-Mejia
Ejercicios 
[Ejercicios Dasha.txt](https://github.com/user-attachments/files/31199226/Ejercicios.Dasha.txt)
Ejercicio

1. ¿Cuántos individuos hay?
# nrow(plantas)
[1] 8

2. ¿Cuántas variables hay?
# length(plantas)
[1] 5

3. Obtén todas las alturas.
#plantas$altura
[1] 12  8 15 20  7 18 11 14

4. Obtén todos los diámetros.
# plantas$diametro
[1] 25 18 32 40 15 35 22 28

5. Obtén solamente los pinos.
#plantas[plantas$especie == "Pino", ]
  individuo especie altura diametro sitio
1         1    Pino     12       25     A
3         3    Pino     15       32     B
6         6    Pino     18       35     C


6. Obtén solamente los encinos.
#> plantas[plantas$especie == "Encino", ]
  individuo especie altura diametro sitio
2         2  Encino      8       18     A
5         5  Encino      7       15     C
8         8  Encino     14       28     B



7. Obtén los individuos del sitio A.
# plantas[plantas$sitio == "A", ]
  individuo especie altura diametro sitio
1         1    Pino     12       25     A
2         2  Encino      8       18     A
7         7  Oyamel     11       22     A



8. Obtén los individuos con altura > 10.
#plantas[plantas$altura>10,]
  individuo especie altura diametro sitio
1         1    Pino     12       25     A
3         3    Pino     15       32     B
4         4  Oyamel     20       40     B
6         6    Pino     18       35     C
7         7  Oyamel     11       22     A
8         8  Encino     14       28     B



9. Obtén los individuos con diámetro > 25.
#plantas[plantas$diametro>25,]
  individuo especie altura diametro sitio
3         3    Pino     15       32     B
4         4  Oyamel     20       40     B
6         6    Pino     18       35     C
8         8  Encino     14       28     B



10. Obtén los pinos con altura > 15.
# plantas[plantas$especie == "Pino" & plantas$altura > 15,]
  individuo especie altura diametro sitio
6         6    Pino     18       35     C


11. Obtén los árboles del sitio B con diámetro > 30.
# plantas[plantas$sitio == "B"& plantas$diametro>30,]
  individuo especie altura diametro sitio
3         3    Pino     15       32     B
4         4  Oyamel     20       40     B


12. Cambia la altura del individuo 5 a 9.
# plantas$altura[5]<-9
 plantas
  individuo especie altura diametro sitio
1         1    Pino     12       25     A
2         2  Encino      8       18     A
3         3    Pino     15       32     B
4         4  Oyamel     20       40     B
5         5  Encino      9       15     C
6         6    Pino     18       35     C
7         7  Oyamel     11       22     A
8         8  Encino     14       28     B



13. Crea una columna altura_cm.
# plantas$altura_cm=plantas$altura*100
> plantas
  individuo especie altura diametro sitio altura_cm
1         1    Pino     12       25     A      1200
2         2  Encino      8       18     A       800
3         3    Pino     15       32     B      1500
4         4  Oyamel     20       40     B      2000
5         5  Encino      9       15     C       900
6         6    Pino     18       35     C      1800
7         7  Oyamel     11       22     A      1100
8         8  Encino     14       28     B      1400





14. Calcula la altura promedio.
# mean(plantas$altura)
[1] 13.375



15. Calcula el diámetro máximo.
# max(plantas$diametro)
[1] 40





