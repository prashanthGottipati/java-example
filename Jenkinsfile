pipeline{
	agent {label 'tomcatSlave2'}
	parameters {
 		 string defaultValue: 'example', name: 'test'
	}
	stages{
        stage('Build stage') {
            steps {
                echo 'This is a build stage'
				sh 'sleep 5'
		    		echo 'Testing TomcatSlave2 *****'
			}
		}
        stage('Push stage') {
            steps {
                echo 'This is push stage'
                sh 'sleep 5'
		echo 'Checking Webhook trigger ***********'
		echo 'Checking Webhook trigger  2nd time ***********'
			}
		}
        stage('Deploy stage') {
            steps {
                echo 'This is deploy stage'
                sh 'sleep 5'
			}
		}
	}
}	
