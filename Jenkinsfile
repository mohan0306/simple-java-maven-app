
currentBuild.displayName = "simple-java-maven-app-#"+currentBuild.number
pipeline{
    agent any
    
    stages {
        stage('continuous download') {
            steps {
                git 'https://github.com/mohan0306/simple-java-maven-app.git'
            }
               
        }
        stage('continuous build') {
            steps {
                sh 'mvn clean install'
            }
        }
            stage('continuous deploy') {
            steps {
                sh 'cp /root/.jenkins/workspace/Demo_tomcat/gameoflife-web/target/gameoflife.war /mnt/apache-tomcat-9.0.71/webapps'
//                 sh 'cp /root/.jenkins/workspace/Game_Of_life/gameoflife-web/target/gameoflife.war /home/ansible'
//              sh 'scp /root/.jenkins/workspace/Game_Of_life/gameoflife-web/target/gameoflife.war ansible@172.31.86.205:/mnt'
            }
               
        }
}
   
}
