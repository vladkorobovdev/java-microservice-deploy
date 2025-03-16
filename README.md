# java-microservice-deploy

### To start the whole project you should run these commands:<br />
#### For linux:  
1. cd service-one
   ./mvnw clean package
   - INFO: Cleans the project by removing old build artifacts. Compiles the source code. Runs tests (if configured). Packages the project into an artifact (like a JAR or WAR file).
2. cd service-two
   ./mvnw clean package
3. cd service-three
   ./mvnw clean package
4. docker-compose up --build (or docker-compose up if nothing changed)  
   - INFO: --build option forces Docker Compose to rebuild the images for the services before starting the containers. It is useful when you have made changes to the Dockerfile or the application code and want to ensure that the latest version of the image is built before the containers start

#### For windows:
1. cd service-one
   .\mvnw.cmd clean package (or mvnw clean package)
2. cd service-two
   .\mvnw.cmd clean package
3. cd service-three
   .\mvnw.cmd clean package
4. docker-compose up --build (or docker-compose up if nothing changed)  