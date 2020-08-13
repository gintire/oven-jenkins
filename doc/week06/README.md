# 7장 젠킨스를 이용한 CI

https://github.com/nikhilpathania/hello-world-greeting

### 브랜치 전략
- master
- develop (mainline)
- feature

## CI JenkinsFile

### Build && Test
- DskipITs=true : 통합 테스트를 생략하고 빌드와 단위테스트만 진행
- surefilre-reports : 단위 테스트의 결과물 위치로 젠킨스에 올리게 된다.

### Static Code Analysis
- Dsonar.projectName : 소나큐브 프로젝트 명 
- Dsonar.projectVersion : 젠킨스 빌드 넘버

### Integration Test
- Dsurefire.skip=true : 단위 테스트를 건너뛰고 통합 테스트만 수행한다.

### Publish

Default Artifactory server : 젠킨스에 설치된 아티팩토리 서버 명칭이다. 