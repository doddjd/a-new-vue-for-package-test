pipeline {
  agent any
  stages {
    stage('') {
      steps {
        sh '''cd $WORKSPACE
yarn install
rm -rf dist/
rm -f webapp_test.zip
yarn run build
cd dist
cp -r ./* /opt/static_file/vue/
rm -rf ./*'''
      }
    }
  }
}