pipeline{
    tools { 
        maven 'maven-3.8.1' 
       
    }
    agent {
        label 'build-agent'
        }
        stages{
            stage('git stage'){
                steps{
                    git branch: 'main', url: 'https://github.com/cloudtechmasters/springboot-maven-course-micro-svc.git'
                }
            }
            stage('build maven project '){
                steps{
                   sh 'mvn clean package'
                }
            }
        }
}
