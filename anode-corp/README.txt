1. to compile and deploy the project:
   mvn clean install
2. change the BAE app id 
   in file : pom.xml
    <plugin>
        <groupId>com.baidu.bae.maven</groupId>
        <artifactId>bae-maven-plugin</artifactId>
        <version>1.0.0.0</version>
        <executions>
        	<execution>
        		<id>baedeploy</id>
        		<phase>install</phase>
        		<goals>
        			<goal>baedeploy</goal>
        		</goals>
        		<configuration>
        			<changepass>false</changepass>
        			<appid>your_app_id</appid>
        			<version>0</version>     			
        		</configuration>
        	</execution>
        </executions>
    </plugin> 
    
3. to run it in local jetty
   mvn baejetty:run
   
   
TODO :

1. add spring mvc
2. add hibernate with mysql configuration.
