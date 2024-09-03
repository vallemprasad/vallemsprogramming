Project Name: Create jenkins pipeline project
Reference: https://www.jenkins.io/doc/pipeline/tour/hello-world/

Steps:

1. Install jenkins

https://www.jenkins.io/doc/book/installing/war-file/

java -jar jenkins.war-httpPort:8080

2. Install the Docker Pipeline plugin through the Manage Jenkins > Plugins page

3. After installing the plugin, restart Jenkins so that the plugin is ready to use


4. Create git hub account and install git in the machine. As a first time user perform below actions.

i. git config --global user.emai "vallemsprogramming@gmail.com"
ii. git config --global user.name "prasad"
iii. git remote set-url origin git@github.com:vallemprasad/vallemsprogramming.git
iv. Generate Keys at $HOME/.ssh by using command ssh-keygen -t rsa
v. Add id_rsa.pub content of such a public key to your Github account: click your profile photo -> Settings-> SSH and GPG keys -> New SSH key or Add SSH key

5. Copy one of the examples below into your repository and name it Jenkinsfile


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


6. Follow the steps https://www.jenkins.io/doc/pipeline/tour/hello-world/
