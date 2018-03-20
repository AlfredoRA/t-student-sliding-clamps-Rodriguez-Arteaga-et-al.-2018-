# t-student-sliding-clamps-Rodriguez-Arteaga-et-al.-2018-
Data of abundance of amino acids in monomers of sliding clamps

Archive is in: PruebaEst.csv
To Glutamate: 

datos = read.csv(archive) 
dim(datos) 
datos[7,]
datos[7, c(3:11,13,15:20)]
boxplot(as.numeric(datos[4, 3:20]))
organismos = as.numeric(datos[4, c(3:12,14:20)])
t.test(organismos, mean = 11.3, conf.level=0.999)
shapiro.test(organismos)
