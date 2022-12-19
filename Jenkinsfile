pipeline 
{
    agent any
    stages 
    {
        stage("Checkout") 
        {
            steps { git url: 'https://github.com/lokanw/calculator.git', branch: 'main'}
        }
        stage("Compile") 
        {
            steps{Sh “chmod +x gradlew”}
            steps {sh "./gradlew compileJava"}
        }  
    }
}