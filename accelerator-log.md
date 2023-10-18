# Accelerator Log

## Options
```json
{
  "acsRepoLabel" : "main",
  "acsRepoPattern" : "application/default",
  "acsRepoUri" : "https://git-server/app-config-repo",
  "apiDescription" : "Manage customer profiles",
  "apiOwner" : "customer-relations-department",
  "apiSystem" : "profile-management",
  "artifactId" : "customer-profile",
  "buildTool" : "maven",
  "databaseMigrationTool" : "flyway",
  "databaseName" : "postgres-database",
  "enableAppConfigService" : true,
  "exposeOpenAPIEndpoint" : true,
  "groupId" : "com.example",
  "javaVersion" : "11",
  "packageName" : "com.example.customerprofile",
  "projectName" : "asa-java-rest-service"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(GeneratorValidationTransform, UniquePath)
┃ ┏ ┏ engine.transformations[0].validated (Combo)
┃ ┃ ┃  Info Combo running as Let
┃ ┃ ┃ engine.transformations[0].validated.delegate (Let)
┃ ┃ ┃ Debug Adding symbol packageDirectory with value 'com/example/customerprofile'
┃ ┃ ┃ Debug Adding symbol workloadResourceName with value 'customer-profile'
┃ ┃ ┃ Debug Adding symbol databaseResourceName with value 'postgres-database'
┃ ┃ ┃ Debug Adding symbol workloadJavaVersion with value '11'
┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Exclude)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[0] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#buildTool == 'maven') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[0].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Exclude, Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[0] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle.kts matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.jar matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.properties matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug gradle.properties matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew.bat matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug settings.gradle.kts matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**, gradle.properties] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[1] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[1].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[1].sources[0].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[1].sources[0].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[1].sources[0].delegate.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [pom.xml, README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [pom.xml, README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml, README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug src/test/resources/application-test.properties didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[1].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[1].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[1].sources[1].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[1].sources[1].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace [<groupId>com.vmware.tap.accelerators</groupId>-><groupId>com.example...(truncated)]
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[1].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[1].sources[2].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[1].sources[2].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[1].sources[2].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace regex '--- StartGradle[\s\S]+?--- EndGradle' with ''
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[1].sources[2].delegate.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace regex '--- StartMaven\s|--- EndMaven\s' with ''
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[0].delegate.transformations[2] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[1] (Combo)
┃ ┃ ┃ ┃ ┗  Info Condition (#buildTool == 'gradle') evaluated to false
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[2] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#enableAppConfigService == true) evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[2].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[2].delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[2].delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[2].delegate.transformations[0].sources[0].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[2].delegate.transformations[0].sources[0].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[2].delegate.transformations[0].sources[0].delegate.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug manifest.yaml didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[2].delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#enableAppConfigService) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[2].delegate.transformations[0].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[2].delegate.transformations[0].sources[1].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[2].delegate.transformations[0].sources[1].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [app-config-name->customer-profile-con...(truncated), acs-repo-pattern->application/default, acs-repo-uri->https://git-server/a...(truncated), acs-repo-label->main]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[2].delegate.transformations[0].sources[1].delegate.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace regex '--- StartACS\s|--- EndACS\s' with ''
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[2].delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[3] (Combo)
┃ ┃ ┃ ┃ ┗  Info Condition (!#enableAppConfigService) evaluated to false
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[4] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[4].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Exclude, Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[0] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [src/main/resources/db/**]
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [src/main/resources/db/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml matched [src/main/resources/db/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql matched [src/main/resources/db/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [src/main/resources/db/**] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[0].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[0].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[0].delegate.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml matched [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml matched [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug manifest.yaml didn't match [pom.xml, build.gradle.kts, **/application.properties, catalog/**, config/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[1].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[1].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '<dependency>\s+<groupId>org\.liquibase</groupId>\s+<artifactId>liquibase-core</artifactId>\s+</dependency>\s+' with ''
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[2].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[2].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [build.gradle.kts]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[2].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace [    implementation("org.liquibase:liquibase-core")->]
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[3].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, OpenRewriteRecipe, OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[3].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/application.properties]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[3].delegate.transformations[1] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[1].sources[3].delegate.transformations[2] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[4].delegate.transformations[2] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[5] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[5].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[5].delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[5].delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[5].delegate.transformations[0].sources[0].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[5].delegate.transformations[0].sources[0].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[5].delegate.transformations[0].sources[0].delegate.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug manifest.yaml didn't match [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[5].delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[5].delegate.transformations[0].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[5].delegate.transformations[0].sources[1].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[5].delegate.transformations[0].sources[1].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [java-version->11, db-server->postgres-database, app-name->customer-profile]
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[5].delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[6] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[6].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[6].delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[6].delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[6].delegate.transformations[0].sources[0].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[6].delegate.transformations[0].sources[0].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[6].delegate.transformations[0].sources[0].delegate.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [config/workload-basic.yaml, config/workload-api-provider.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug manifest.yaml didn't match [config/workload-basic.yaml, config/workload-api-provider.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[6].delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#exposeOpenAPIEndpoint) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[6].delegate.transformations[0].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[6].delegate.transformations[0].sources[1].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/workload-api-provider.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [config/workload-api-provider.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[6].delegate.transformations[0].sources[1].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#exposeOpenAPIEndpoint) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [DESCRIPTION_VAL->Manage customer prof...(truncated), OWNER_VAL->customer-relations-d...(truncated), SYSTEM_VAL->profile-management]
┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[6].delegate.transformations[0].sources[1].delegate.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[6].delegate.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (!#exposeOpenAPIEndpoint) evaluated to false
┃ ┃ ┃ ┃ ┃ ┗ ┗ null ()
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[6].delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[7] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[7].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[7].delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[7].delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Exclude
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[7].delegate.transformations[0].sources[0].delegate (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [config/workload.yaml, config/test-pipeline.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [config/workload.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[7].delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[7].delegate.transformations[0].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[7].delegate.transformations[0].sources[1].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/workload.yaml, config/test-pipeline.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [config/workload.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[7].delegate.transformations[0].sources[1].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [rest-service-db->customer-profile]
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[7].delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[8].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[0].delegate (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[1].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[1].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '<java.version>.*<' with '<java.version>11<'
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[2].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[2].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [build.gradle.kts]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[2].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '(?<unmodified>JavaVersion\.VERSION_)(\d+)' with '${unmodified}11'
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[3].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[3].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/workload.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[3].delegate.transformations[1] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[4].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[4].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/*.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[4].delegate.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will exclude [config/workload.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[0].sources[4].delegate.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace regex '(?<unmodified>image: bellsoft/liberica-openjdk-\w*:)(\d+)' with '${unmodified}11'
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[8].delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┗ ┗ Debug Multiple representations for path 'pom.xml', will use the one appearing last 
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[9].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[0].delegate (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[1].delegate (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [docker-compose-postgresql.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml matched [docker-compose-postgresql.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug pom.xml didn't match [docker-compose-postgresql.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[2].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Combo, OpenRewriteRecipe, OpenRewriteRecipe, OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[2].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [src/main/resources/application-local.properties]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [src/main/resources/application-local.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug pom.xml didn't match [src/main/resources/application-local.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[2].delegate.transformations[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[2].delegate.transformations[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[2].delegate.transformations[1].delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[2].delegate.transformations[1].delegate.transformations[0].sources[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[2].delegate.transformations[1].delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[2].delegate.transformations[2] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[2].delegate.transformations[3] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[2].delegate.transformations[4] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[3].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Combo, OpenRewriteRecipe, OpenRewriteRecipe, OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[3].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [src/test/resources/application-test.properties]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties matched [src/test/resources/application-test.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug pom.xml didn't match [src/test/resources/application-test.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[3].delegate.transformations[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[3].delegate.transformations[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[3].delegate.transformations[1].delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[3].delegate.transformations[1].delegate.transformations[0].sources[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[3].delegate.transformations[1].delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[3].delegate.transformations[2] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[3].delegate.transformations[3] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[3].delegate.transformations[4] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[4].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[4].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/workload.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug pom.xml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[4].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [postgres-database->postgres-database]
┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[4].delegate.transformations[2] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[5] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[5].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[5].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[5].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace regex '(?<startOfDependencies><dependencies>)(?<existingDependencies>(?![\s\S]+<groupId>org.postgresql</groupId>\s*<artifactId>postgresql</artifactId>[\s\S]+</dependencies>))' with '${startOfDependencie...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[5].delegate.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '(?<startOfDependencies><dependencies>)(?<existingDependencies>(?![\s\S]+<groupId>org.testcontainers</groupId>\s*<artifactId>postgresql</artifactId>[\s\S]+</dependencies>))' with '${startOfDependencie...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[6] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[6].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[6].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [build.gradle.kts]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug pom.xml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[6].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace regex '(?<startOfDependencies>dependencies \{)(?<existingDependencies>(?![\s\S]+implementation\s*\("org.postgresql:postgresql[\s\S]+))' with '${startOfDependencie...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[6].delegate.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '(?<startOfDependencies>dependencies \{)(?<existingDependencies>(?![\s\S]+testImplementation\s*\("org.testcontainers:postgresql[\s\S]+))' with '${startOfDependencie...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[7] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[7].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Combo, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[7].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug pom.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[7].delegate.transformations[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[7].delegate.transformations[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[7].delegate.transformations[1].delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[7].delegate.transformations[1].delegate.transformations[0].sources[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[7].delegate.transformations[1].delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[0].sources[7].delegate.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will replace regex '(?<existingContent>[\s\S]*)(?<endOfFile>
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info )' with '${existingContent}
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info 
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info ...(truncated)'
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[9].delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ Debug Multiple representations for path 'pom.xml', will use the one appearing last 
┃ ┃ ┃ ┃ ┃ ┃ Debug Multiple representations for path 'docker-compose-postgresql.yaml', will use the one appearing last 
┃ ┃ ┃ ┃ ┃ ┃ Debug Multiple representations for path 'README.md', will use the one appearing last 
┃ ┃ ┃ ┃ ┃ ┃ Debug Multiple representations for path 'src/test/resources/application-test.properties', will use the one appearing last 
┃ ┃ ┃ ┃ ┗ ┗ Debug Multiple representations for path 'src/main/resources/application-local.properties', will use the one appearing last 
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[10] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[10].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[10].delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[10].delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Exclude
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[10].delegate.transformations[0].sources[0].delegate (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [**/*.java]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/main/resources/application-local.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[10].delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Let
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[10].delegate.transformations[0].sources[1].delegate (Let)
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Adding symbol packageDirectory with value 'com/example/customerprofile'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[10].delegate.transformations[0].sources[1].delegate.in (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[10].delegate.transformations[0].sources[1].delegate.in.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/*.java]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/main/resources/application-local.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[10].delegate.transformations[0].sources[1].delegate.in.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [com.vmware.tap.accelerators.restservicedb->com.example.customer...(truncated)]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[10].delegate.transformations[0].sources[1].delegate.in.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=test, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/api/CustomerProfileControllerTest.java, g0=src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java, g1=test, g2=com/vmware/tap/accelerators/, g3=/api/CustomerProfileControllerTest.java} and was rewritten to 'src/test/java/com/example/customerprofile//api/CustomerProfileControllerTest.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=test, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/domain/CustomerProfileServiceTest.java, g0=src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java, g1=test, g2=com/vmware/tap/accelerators/, g3=/domain/CustomerProfileServiceTest.java} and was rewritten to 'src/test/java/com/example/customerprofile//domain/CustomerProfileServiceTest.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=test, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/ApplicationTests.java, g0=src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java, g1=test, g2=com/vmware/tap/accelerators/, g3=/ApplicationTests.java} and was rewritten to 'src/test/java/com/example/customerprofile//ApplicationTests.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=main, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/domain/CustomerProfileCreateRequest.java, g0=src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java, g1=main, g2=com/vmware/tap/accelerators/, g3=/domain/CustomerProfileCreateRequest.java} and was rewritten to 'src/main/java/com/example/customerprofile//domain/CustomerProfileCreateRequest.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=main, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/domain/CustomerProfileResponse.java, g0=src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java, g1=main, g2=com/vmware/tap/accelerators/, g3=/domain/CustomerProfileResponse.java} and was rewritten to 'src/main/java/com/example/customerprofile//domain/CustomerProfileResponse.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=main, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/api/CustomerProfileController.java, g0=src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java, g1=main, g2=com/vmware/tap/accelerators/, g3=/api/CustomerProfileController.java} and was rewritten to 'src/main/java/com/example/customerprofile//api/CustomerProfileController.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=test, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/data/CustomerProfileRepositoryTest.java, g0=src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java, g1=test, g2=com/vmware/tap/accelerators/, g3=/data/CustomerProfileRepositoryTest.java} and was rewritten to 'src/test/java/com/example/customerprofile//data/CustomerProfileRepositoryTest.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=main, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/data/CustomerProfileEntity.java, g0=src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java, g1=main, g2=com/vmware/tap/accelerators/, g3=/data/CustomerProfileEntity.java} and was rewritten to 'src/main/java/com/example/customerprofile//data/CustomerProfileEntity.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=main, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/domain/CustomerProfileChangeRequest.java, g0=src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileChangeRequest.java, g1=main, g2=com/vmware/tap/accelerators/, g3=/domain/CustomerProfileChangeRequest.java} and was rewritten to 'src/main/java/com/example/customerprofile//domain/CustomerProfileChangeRequest.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=main, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/Application.java, g0=src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java, g1=main, g2=com/vmware/tap/accelerators/, g3=/Application.java} and was rewritten to 'src/main/java/com/example/customerprofile//Application.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=main, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/domain/CustomerProfileService.java, g0=src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java, g1=main, g2=com/vmware/tap/accelerators/, g3=/domain/CustomerProfileService.java} and was rewritten to 'src/main/java/com/example/customerprofile//domain/CustomerProfileService.java'
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗ ┗ Debug Path 'src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=main, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/data/CustomerProfileRepository.java, g0=src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java, g1=main, g2=com/vmware/tap/accelerators/, g3=/data/CustomerProfileRepository.java} and was rewritten to 'src/main/java/com/example/customerprofile//data/CustomerProfileRepository.java'
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[10].delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[11] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[11].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[11].delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[11].delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[11].delegate.transformations[0].sources[0].delegate (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/*.jar]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileService.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/Application.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileResponse.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/domain/CustomerProfileServiceTest.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileEntity.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/api/CustomerProfileController.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/api/CustomerProfileControllerTest.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileCreateRequest.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileRepository.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/data/CustomerProfileRepositoryTest.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileChangeRequest.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/ApplicationTests.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[11].delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.in.transformations[11].delegate.transformations[0].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Exclude, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[11].delegate.transformations[0].sources[1].delegate.transformations[0] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [**/*.jar]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileService.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/Application.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileResponse.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/domain/CustomerProfileServiceTest.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileEntity.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/api/CustomerProfileController.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/api/CustomerProfileControllerTest.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileCreateRequest.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileRepository.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/data/CustomerProfileRepositoryTest.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileChangeRequest.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/ApplicationTests.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[11].delegate.transformations[0].sources[1].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [rest-service-db->customer-profile]
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.in.transformations[11].delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.in.transformations[12] (Exclude)
┃ ┃ ┃ ┃ ┃  Info Will exclude [manifest.yaml]
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileService.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileResponse.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/Application.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/domain/CustomerProfileServiceTest.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/api/CustomerProfileController.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileEntity.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/api/CustomerProfileControllerTest.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileCreateRequest.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug DATABASE.md didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/data/CustomerProfileRepositoryTest.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileRepository.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug docker-compose-postgresql.yaml didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileChangeRequest.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/ApplicationTests.java didn't match [manifest.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [manifest.yaml] -> included
┃ ┗ ┗ ┗ ┗ Debug manifest.yaml matched [manifest.yaml] -> excluded
┗ ╺ engine.transformations[1] (UniquePath)
```
