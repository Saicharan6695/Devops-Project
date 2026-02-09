pipeline {

agent any 

options{
skipDefaultCheckout()
}

environment{

APP_NAME = "MyDemoApp"
ENV_TYPE = 'QA'

}


parameters{

string(name: 'MESSAGE' , defaultValue: 'Hello from Pipeline' , description: 'message to print' )

}

stages{

stage('checkout') {

steps{

checkout scm

}
}

stage('Test'){

steps{

echo 'Test phase is running' 

}
}

stage('Build'){

steps{

echo 'Build phase is running'

}
}

}
}