# basic-java-project

Proyecto Java basico pensado como punto de partida para practicar una CI sencilla con GitHub Actions.

## Estructura

```text
basic-java-project/
	pom.xml
	src/
		main/java/com/vodafone/basic/App.java
		test/java/com/vodafone/basic/AppTest.java
```

## Requisitos

- Java 17
- Maven 3.9+

Alternativa recomendada:

- Dev Container de VS Code (ya incluido en `.devcontainer/devcontainer.json`)

## Ejecutar en local

Compilar y ejecutar tests:

```bash
mvn clean verify
```

Ejecutar la aplicacion:

```bash
mvn -q exec:java -Dexec.mainClass="com.vodafone.basic.App"
```

Salida esperada:

```text
Hello world!
```

## Desarrollo con Dev Container

1. Abre la carpeta en VS Code.
2. Ejecuta el comando: `Dev Containers: Reopen in Container`.
3. El contenedor instala el entorno y lanza un test basico automaticamente.

## Idea de CI basica

Para un workflow inicial de GitHub Actions, el becario puede empezar con estos pasos:

1. Checkout del repositorio.
2. Setup de Java 17.
3. Cache de dependencias Maven.
4. `mvn -B clean verify`.
