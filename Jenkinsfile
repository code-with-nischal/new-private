node {
    def mavenHome = tool name: 'maven-1'
echo "the node name is : -->${env.NODE_NAME}"

echo "the job name is : --> ${env.JON_NAME}"

echo "this build no is : --> ${env.BUILD_NUMBER}"

properties([buildDiscarder(logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '', numToKeepStr: '5'))])
    stage('checkout code') {
        git branch: 'master',
            credentialsId: 'git',
            url: 'https://github.com/code-with-nischal/new-private.git'
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
