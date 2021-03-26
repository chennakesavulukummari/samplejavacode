pipeline {
    agent any 
    stages {
        stage('Stage-1 : Clean') { 
            steps {
                withMaven(maven : 'maven'){
                    sh 'mvn clean'
                } 
            }
        }
        stage('Stage-2 : Validate') { 
            steps {
                withMaven(maven : 'maven'){
                    sh 'mvn validate'
                } 
            }
        }
        stage('Stage-3 : Compile') { 
            steps {
                withMaven(maven : 'maven'){
                    sh 'mvn compile'
                } 
            }
        }
        stage('Stage-4 : Test') { 
            steps {
                withMaven(maven : 'maven'){
                    sh 'mvn test -DskipTests'
                } 
            }
        }
       /* stage('Stage-5 : Install') { 
            steps {
                withMaven(maven : 'maven'){
                    sh 'mvn install -DskipTests'
                } 
            }
        }
        stage('Stage-6 : Verify') { 
            steps {
                withMaven(maven : 'maven'){
                    sh 'mvn verify -DskipTests'
                } 
            }
        }
        stage('Stage-7 : Package') { 
            steps {
                withMaven(maven : 'maven'){
                    sh 'mvn package -DskipTests'
                } 
            }
        }
        stage('Stage-8 : Deploy an Artifact to Artifactory Manager i.e. Nexus/Jfrog') { 
            steps {
                withMaven(maven : 'maven'){
                    sh 'mvn deploy -DskipTests'
                } 
            }
        }
        stage('Stage-9 : Deployment - Deploy a Artifact codewithck-1.0.0-SNAPSHOT.war file to Tomcat Server '){
            steps{
                sh 'curl -u admin:Azure@2021 -T target/**.war "http://192.168.29.67:8080/manager/text/deploy?path=/codewithck&update=true"' 
            }
        }
        stage('Stage-10 : SmokeTest'){
            steps{
                sh 'curl --retry-delay 10 --retry 5 "http://192.168.29.67:8080/codewithck"' 
            }
        }*/
    }
}
