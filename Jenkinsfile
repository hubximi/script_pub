node {
  stage ('run scanner') {
    sh 'docker run -e API_BASE_URL=https://tron.cust02.int.tronsec.ru/ -e SKIP_API_SERVER_VALIDATION=true -e API_TOKEN=${API_TOKEN} -e COMPANY_EXT_REGISTRY_USERNAME=${COMPANY_EXT_REGISTRY_USERNAME} -e COMPANY_EXT_REGISTRY_PASSWORD=${COMPANY_EXT_REGISTRY_PASSWORD} ximilab.gitlab.yandexcloud.net:5050/ximidev/tron/scanner:v1.1.0-with-db jfrog.tronsec.ru/demo-tron/bad:bad-project-test --html --stdout > result.html'
  }
}	
