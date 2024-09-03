Project Name: Create jenkins pipeline project
Reference: https://www.jenkins.io/doc/pipeline/tour/hello-world/

Steps:

1. Install jenkins

https://www.jenkins.io/doc/book/installing/war-file/

java -jar jenkins.war-httpPort:8080

2. Install the Docker Pipeline plugin through the Manage Jenkins > Plugins page

3. After installing the plugin, restart Jenkins so that the plugin is ready to use

4. Copy one of the examples below into your repository and name it Jenkinsfile


Jenkinsfile (Declarative Pipeline)

/* Requires the Docker Pipeline plugin */
pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}


5. Follow the steps https://www.jenkins.io/doc/pipeline/tour/hello-world/
