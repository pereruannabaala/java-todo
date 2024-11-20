pipeline{
    agent any
    
    tools{
        gradle 'gradle'
    }
    
    stages{
        
        stage("Clone Repo"){
            steps{
                git branch:'master', url:'https://github.com/kadimasum/java-todo'
            }
        }
        
        stage("Build Code"){
            steps{
                sh 'gradle build'
            }
        }
        
        stage("Test Code"){
            steps{
                sh "gradle test"
            }
        }
    }
}