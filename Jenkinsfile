pipeline{
	agent any
	stages{
		stage('git'){
		  steps{
			git 'https://github.com/BhatiLakhansingh/game-of-life.git'
			}
		}
		stage('build'){
		   steps{
			sh 'mvn package'
			}
		}
	}
}
