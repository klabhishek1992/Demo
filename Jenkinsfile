pipeline 
{
    agent any
   	 stages 
    {
        stage('Build') 
        {
            steps 
            {
                echo 'This is to build App'
            }
       	}
    stage('Test') 
        {
            steps 
            {
                echo 'This is to Test App'
            }
       	}
    stage('Deploy') 
        {
            steps 
            {
                echo 'This is to Deploy App'
            }
       	}
    }
    post 
    {
 	    always 
        {
            emailext body: 'Summary', replyTo: 'klabhishek1992@gmail.com', subject: 'Pipe Notify', to: 'klabhishek1992@gmail.com'
	    }
    }

}
