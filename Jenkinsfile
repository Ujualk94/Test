pipeline{
    agent any
    
    environment{
        PATH = "/bin/mvn:$PATH"
    stages{
        stage("Git checkout"){
            steps{
                git 'https://github.com/javahometech/myweb'
            }
        }
        stage("maven build"){
            steps{
                sh "mvn clean package"
            }
        }          
    }
}
