pipeline{
    agent any
    stage('Checkout') {
         steps {
             echo ">>>>>>>> Checkout branch ${params.BRANCH}"
         }
    }
    stage('Install') {
         steps {
             echo ">>>>>>>> Install ${params.INSTALL}..."
             sh "cd ${WORKSPACE}"
             sh 'npm config set registry=https://registry.npm.taobao.org'
             sh 'npm install'
         }
    }

}