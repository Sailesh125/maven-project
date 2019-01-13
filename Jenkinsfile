pipeline{
agent any
stages{
stage('build'){
steps{
sh 'mvn clean package'
}
post{
sucess{
echo 'now arching'
archiveArtifacts artifacts: '**/target/*.war'
}
}
}
}
}
