node {
    def mavenHome = tool name: 'maven-1'

    stage('checkout code') {
        git branch: 'master',
            credentialsId: 'git',
            url: 'https://github.com/code-with-nischal/testing.git'
    }


//build stage
/*
stage('build'){

sh "$mavenHome/bin/mvn clean package"
}
//deploy stage
stage('deploy'){
sshagent([]) {
 sh "scp -o StrictHostKeyChecking=no target/maven-web-application.war ec2-user@3.235.225.165:/opt/apache-tomcat-11.0.14/webapps" 
}
}
*/
}
