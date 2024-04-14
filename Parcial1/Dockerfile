# imagen maven
FROM maven:3.9.6-eclipse-temurin-17-focal AS build

# Fijar el directorio de trabajo dentro del contenedor
WORKDIR /app

# Transferir el archivo pom.xml al directorio de trabajo del contenedor
COPY pom.xml .

# Copia lo demas del código fuente al directorio de trabajo del contenedor
COPY src ./src

# Compila la aplicación utilizando Maven
RUN mvn clean package -DskipTests

# proceso numero dos del Dockerfile para su ejecucion
FROM maven:3.9.6-eclipse-temurin-17-focal

# Establece el directorio de trabajo dentro del contenedor
WORKDIR /app

# Transferir exclusivamente el archivo JAR previamente compilado desde la fase de compilación anterior al directorio de trabajo del contenedor."
COPY --from=build /app/target/crud-0.0.1-SNAPSHOT.jar java-app.jar

# Definir el comando de arranque para ejecutar la aplicación
ENTRYPOINT ["java", "-jar", "java-app.jar"]
