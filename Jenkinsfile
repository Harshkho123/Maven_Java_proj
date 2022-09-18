pipeline{
    agent any
    parameters{
        choice(name: 'Version', choices: ['1.2','1.3','1.4'], description:'')
    }
    stages{
        stage("Build"){
            steps{ 
                when{
                  expression{
                     params.Version == 1.2
                }
            }
                echo "Build the stage"
            }
            }
stage("Test")
{
    steps{
        echo "show the version: ${Version}"
    }
}
    }
    
}
