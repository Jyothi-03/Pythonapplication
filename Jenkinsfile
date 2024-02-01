pipeline{
  agent any
  parameters{
    choice(choices:["Add","Subtract","multiply","Divide"], description: "Select ur choice", name: "operation")
    string(defaultValue: "", description: "Enter your first number here", name: "firstnumber")
    string(defaultValue: "", description: "Enter your second number here", name: "secondnumber")
  }
  stages{
    stage('Build'){
      steps{
        sh "python3 main.py ${params.operation} ${params.firstnumber} ${params.secondnumber}'"
      }
    }
  }
}

    
      
      

