def workspace;
node
{
    stage('Checkout')
    {
       checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'b4d55905-c64c-462f-a2f4-e16565579bae', url: 'https://github.com/velychkov/Learning_Jenkins.git']]])
       workspace =pwd()
    }
    stage('Static Code Analysis')
    {
        echo "Static code analysis"
    }
    stage('Build')
    {
        echo "Build the code"
    }
    stage('Unit testing')
    {
        echo "Unit testing"
    }
    stage ('Delivery')
    {
        echo "Delivery the code"
    }
}
