pipeline {
    // where or who
    agent any
    
    // collection of stages
    stages{
        stage('Test'){
            steps{
                echo 'test'
            }
        }
        stage('Package'){
            steps{
	        echo 'Package'
               
            }
        }
        stage('Deploy war'){
            steps{
                echo 'Deploy'
            }
        }
    }
    post{
        failure{
            echo 'Build failed'
        }
        success{
            echo 'Build Success'
        }
    }
}
