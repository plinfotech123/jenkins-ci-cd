// pipeline{
//     agent any
//
//     tools{
//         maven "maven"
//     }
//
//     stages{
//
//         stage("SCM checkout"){
//             steps{
//                 checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/javatechie-devops/jenkins-ci-cd.git']])
//             }
//         }
//
//         stage("Build Process"){
//             steps{
//                 script{
//                     sh 'mvn clean install'
//                 }
//             }
//         }
//
//
//
//
//     }
//
//     post{
//         always{
//             emailext attachLog: true,
//             body: ''' <html>
//     <body>
//         <p>Build Status: ${BUILD_STATUS}</p>
//         <p>Build Number: ${BUILD_NUMBER}</p>
//         <p>Check the <a href="${BUILD_URL}">console output</a>.</p>
//     </body>
// </html>''', mimeType: 'text/html', replyTo: 'javatechie.learning@gmail.com', subject: 'Pipeline Status : ${BUILD_NUMBER}', to: 'javatechie.learning@gmail.com'
//
//         }
//     }
// }
//
// //SCM checkout
// //build
// //deploy WAR
// // EMAIL