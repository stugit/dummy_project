pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                /* `make check` returns non-zero on test failures,
                * using `true` to allow the Pipeline to continue nonetheless
                */
                sh 'date'
                print "DEBUG: parameter payload = ${payload}"
                echo "Running build ${env.BUILD_ID} on ${env.JENKINS_URL}"                
                sh 'git tag'
                sh 'git clone -b v0.0.1 https://github.com/stugit/dummy_project.git'
                sh 'env'
            }
        }
        stage('Integration Testing') {
            steps {
                /* `make check` returns non-zero on test failures,
                * using `true` to allow the Pipeline to continue nonetheless
                */
                print "DEBUG: parameter payload = ${payload}"
                echo "Running build ${env.BUILD_ID} on ${env.JENKINS_URL}"                
            }
        }
        stage('Build Artifacts') {
            steps {
                /* `make check` returns non-zero on test failures,
                * using `true` to allow the Pipeline to continue nonetheless
                */
                print "DEBUG: parameter payload = ${payload}"                
            }
        } 
        stage('Deploy Artifacts') {
            steps {
                /* `make check` returns non-zero on test failures,
                * using `true` to allow the Pipeline to continue nonetheless
                */
                print "DEBUG: parameter payload = ${payload}"                 
            }
        }          
        
        
        stage('Housekeeping') {
            steps {
                /* `make check` returns non-zero on test failures,
                * using `true` to allow the Pipeline to continue nonetheless
                */
                print "DEBUG: parameter payload = ${payload}"                 
            }
        }              
    }
}
