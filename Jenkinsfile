pipeline 
{
    agent any

    stages 
    {
        stage('Built') 
        {
            steps 
            {
                echo 'Hello Built'
            }
        }
        stage('Testing') 
        {
            steps 
            {
                echo 'Happy Testing'
            }
        }
        stage('Deploy') 
        {
            steps 
            {
                echo 'Finally Deploy'
            }
        }
    }
    post
    {
        always
        {
            emailext body: 'Summary', subject: 'Pipeline status', to: 'dash.subhankar85@gmail.com'
        }
    }
}    
