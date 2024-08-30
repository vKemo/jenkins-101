pipeline {
    agent { none }  // No agent allocated for the entire pipeline

    stages {
        stage('Build') {
            agent { label 'my-agent-label' }  // Specify an agent for this stage
            steps {
                echo "Building.."
                sh '''
                echo "doing build stuff.."
                '''
            }
        }
        stage('Test') {
            agent { label 'my-agent-label' }  // Specify an agent for this stage
            steps {
                echo "Testing.."
                sh '''
                echo "doing test stuff.."
                '''
            }
        }
        stage('Deliver') {
            agent { label 'my-agent-label' }  // Specify an agent for this stage
            steps {
                echo 'Deliver....'
                sh '''
                echo "doing delivery stuff.."
                '''
            }
        }
    }
}
