podTemplate(containers: [containerTemplate(name: 'maven', image: 'maven', command: 'sleep', args: 'infinity')]) {
  node(POD_LABEL) {
    checkout scm
    container('maven') {
      sh 'mvn -B -ntp -Dmaven.test.failure.ignore verify'
    }
 //djhdn teste
    //brb teste 02
    // ect teste 11:47
    junit '**/target/surefire-reports/TEST-*.xml'
  }
}
