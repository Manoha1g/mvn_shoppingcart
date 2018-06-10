
node
{
    stage('Git')
    {
    git 'https://github.com/Manoha1g/mvn_shoppingcart.git'
    
    }
    stage('Build')
    {
       def mvnHome =  tool name: 'Maven3.5', type: 'maven'
       sh "${mvnHome}/bin/mvn clean package"
    }
    stage('Deploy to Tomcat')
    {
        sshagent(['tomcat-server'])
        {
            sh 'scp -o StrictHostKeyChecking=no target/*.war ec2-user@172.31.24.240:/opt/apache-tomcat-9.0.8/webapps/'
        }
    }
}


