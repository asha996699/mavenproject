pipeline
{
    agent any

    stages 
    {
        stage('Build')
        {
            steps
            {
                echo 'Build App'
            }
        }
         stage('Test')
        {
            steps
            {
                echo 'Test App'
            }
        }
         stage('Deploy')
        {
            steps
            {
                echo 'Deploy App'
            }
        }
    }
    
    Post
    { 
      
        always
        {
            emailext body: 'Summary', subject: 'Pipeline Status', to: 'ashadevops.2021@gmail.com'
        }
    }
}
