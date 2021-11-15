pipeline {
    agent any

    stages {
        stage('BuildAndTest') {
            steps {
                bat(script: "powershell -NonInteractive -Command \"& { &'\\\\srv-src\\hg\\dev-config\\Jenkins\\BuildStep.ps1' '%WORKSPACE%' '%JENKINS_HOME%' '%BUILD_URL%' '%JOB_NAME%' '%BUILD_NUMBER%' '%CHANGE_AUTHOR%' '%CHANGE_AUTHOR_EMAIL%' '%CHANGE_AUTHOR_DISPLAY_NAME%'}\"")
            }
        }
    }
}