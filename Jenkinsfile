pipeline{
    agent any
    tools{
        gradle 'gradle'
    }
    stages{
        stage("Clone Repository"){
            steps{
                git branch: 'master', url: 'https://github.com/kadimasum/java-todo.git'
            }
        }
        
        stage("Build Project"){
            steps{
                sh 'gradle build'
            }
        }
        
        stage("Test Project"){
            steps{
                sh 'gradle test'
            }
        }
    }
}