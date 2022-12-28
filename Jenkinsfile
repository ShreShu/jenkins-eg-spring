pipeline{
      stages{

           stage('Repo cloning'){
            steps{
                git credentialsId: 'c55e466b-4e82-4141-bb9d-0fdb40695650', url: 'https://github.com/ShreShu/jenkins-eg-spring'
            }
    }
            stage('version check'){
                steps{
                bat 'mvn -v'
            }
    }
             stage('Build'){
                steps{
                bat 'mvn clean test'
            }
    }
    }
}
