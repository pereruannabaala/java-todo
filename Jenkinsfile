pipeline{
    agent any
    
    tools{
        gradle "gradle"
    }
    
    stages{
        stage("Clone code"){
            steps{
                git branch:"master", url:"https://github.com/kadimasum/java-todo.git"
            }
        }
        
        stage("Build code"){
            steps{
                sh "gradle build"
            }
        }
        
        stage("Test code"){
            steps{
                sh "gradle test"
            }
        }
    }
}