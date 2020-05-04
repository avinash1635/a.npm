pipeline
{
    agent{
        label 'slave'
    } 
    stages
    {
        stage ('continuous download')
        {
            steps
            {
                git 'https://github.com/avinash1635/a.npm.git'
            }
        }
        stage ('continuous build')
        {
            steps
            {
               sh "npm install"
               sh "npm build"                           
            }
        }
    }
}