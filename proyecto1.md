# yakimeshi95
##### PRACTICA 1 ###############
##### 1.- INTRODUCCION A R
# Podemos ocupar R como calculadora
pi # r me genera el numero 
## variables en R
## operaciones aritmeticas
a<-4
b <- 3
a + b
suma <- a + b
suma

#operaciones de comparacion 
a > b # ¿a es mayor que b?
a >- a # a es mayor igual que a
a < b # a es menor que b?
a == b # ¿a es igual que b?
a ==4
a != b # ¿a es diferente a b?

####################

## concepto de funcion 
x <- abs(-2.5) #3 abs es la fucion del valor absoluto 
x
help (abs)
## pedir ayuda en R
help (abs)

## para asignar valores a variables en R se usa una <-
x<-"hola"  ## variable tipo caracter
z <- 6 ## el igual solo funciona en una sola direccion
### En este curso los objetos o variables que se utilizan son de caracter y numerico
ciudad <- "Toluca" # una entrada
nombres <- c("Karla", "Rodrigo", "Miguel", "Samuel") #Caracter y 4 entradas 
edad <- c(28,17,49,31) # numerico y 4 entradas
## se utiliza la uncion class para preguntarle a r que tipo de variables en nombre y edad
class (nombres) ## tipo de variable
class (edad) 

###### PARA CREAR BASE DE DATOS 
base1 <- data.frame (nombres,edad) # se crea una base de datos 
View(base1)   ## ver la base de datos
ls (base1)   ### Ver lista de variables de base 1

base1$edad ###para visualizar solo una variable, edad base 1



#### CREAR UNA VARIABLE DE NOMBRE SEXO CON 4 ENTRADAS 
# donde hombre es 1 y mujer es el valor , la primera entrada es mujere 
# y las otras 3 son hombres
# despues de crear esta variable generen una nueva base
# de nombre base 2 con 3 variables, nombre, edad y sexo 

sexo <- c(2,1,1,1)

base2 <- data.frame(nombres,edad,sexo)
View(base2)
table (base2$sexo) ## contabilizar frecuencia de una variable, sexo.

table (base2$edad)

#####GRAFICAR
palumnos <- c(40,120,60,80) ## alumnos fac economia
etiq <- c("actua","eco", "ri", "neg")
help (pie)

pie (palumnos)
pie (palumnos, etiq)
#titulo de grafica
pie (palumnos,etiq, main =
"Gráfica de pie de la
     facultad de economía",
 sub="Fuente: facultad de economía"
,col = c("blue", "red", "pink", "yellow"),
radius = 1.0,
clockwise = TRUE,
lty = 10)

#para mas tonalidades buscar en colors en R de la universidad de columbia
