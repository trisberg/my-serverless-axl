# Accelerator Log

## Options
```json
{
  "projectName" : "my-serverless-axl",
  "javaVersion" : "21",
  "deploymentType" : "workload",
  "includeBuildToolWrapper" : true,
  "bsGitRepository" : "github.com?owner=trisberg&repo=my-serverless-axl",
  "bsGitBranch" : "main"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(Exclude, GeneratorValidationTransform, UniquePath)
┃ ┏ engine.transformations[0] (Exclude)
┃ ┃  Info Will exclude [accelerator.yaml, accelerator.axl]
┃ ┃ Debug .gitignore didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug LICENSE didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug README.md didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug accelerator.axl matched [accelerator.yaml, accelerator.axl] -> excluded
┃ ┃ Debug accelerator.yaml matched [accelerator.yaml, accelerator.axl] -> excluded
┃ ┃ Debug pom.xml didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug catalog/catalog-info.yaml didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug kubernetes/k8s/DEPLOYING.md didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug kubernetes/k8s/Tiltfile didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug kubernetes/k8s/deployment.yaml didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug kubernetes/k8s/service.yaml didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug kubernetes/tap/.tanzuignore didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug kubernetes/tap/DEPLOYING.md didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug kubernetes/tap/Tiltfile didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug kubernetes/tap/workload.yaml didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug src/main/resources/application.properties didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┏ ┏ engine.transformations[1].validated (Chain)
┃ ┃ ┃  Info Running Chain(IfElse, ApplyTo, Merge, UniquePath, Provenance)
┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[0] (IfElse)
┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[0].otherwise (Chain)
┃ ┃ ┃ ┃  Info Running Chain(IfElse, UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[0].otherwise.transformations[0] (IfElse)
┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[0].otherwise.transformations[0].otherwise (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Exclude, ApplyTo, ApplyTo, ApplyTo, ApplyTo)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[0].otherwise.transformations[0].otherwise.transformations[0] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [kubernetes/k8s/**]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [kubernetes/k8s/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [kubernetes/k8s/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [kubernetes/k8s/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [kubernetes/k8s/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [kubernetes/k8s/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md matched [kubernetes/k8s/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile matched [kubernetes/k8s/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml matched [kubernetes/k8s/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml matched [kubernetes/k8s/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/.tanzuignore didn't match [kubernetes/k8s/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/DEPLOYING.md didn't match [kubernetes/k8s/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/Tiltfile didn't match [kubernetes/k8s/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/workload.yaml didn't match [kubernetes/k8s/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [kubernetes/k8s/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [kubernetes/k8s/**] -> included
┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [kubernetes/k8s/**] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[0].otherwise.transformations[0].otherwise.transformations[1].apply (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[0].otherwise.transformations[0].otherwise.transformations[1].apply.transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [hello-fun->my-serverless-axl]
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[0].otherwise.transformations[0].otherwise.transformations[1].apply.transformations[1] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'kubernetes/tap/workload.yaml' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=.yaml, folder=kubernetes/tap/, filename=workload.yaml, g0=kubernetes/tap/workload.yaml, g1=kubernetes/tap/, g2=workload.yaml, g3=workload.yaml, g4=.yaml} and was rewritten to 'config/workload.yaml'
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[0].otherwise.transformations[0].otherwise.transformations[2].apply (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[0].otherwise.transformations[0].otherwise.transformations[2].apply.transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [hello-fun->my-serverless-axl]
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[0].otherwise.transformations[0].otherwise.transformations[2].apply.transformations[1] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'kubernetes/tap/Tiltfile' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=null, folder=kubernetes/tap/, filename=Tiltfile, g0=kubernetes/tap/Tiltfile, g1=kubernetes/tap/, g2=Tiltfile, g3=Tiltfile, g4=null} and was rewritten to 'Tiltfile'
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[0].otherwise.transformations[0].otherwise.transformations[3].apply (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText, RewritePath, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[0].otherwise.transformations[0].otherwise.transformations[3].apply.transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [hello-fun->my-serverless-axl]
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[0].otherwise.transformations[0].otherwise.transformations[3].apply.transformations[1] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug Path 'kubernetes/tap/DEPLOYING.md' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=.md, folder=kubernetes/tap/, filename=DEPLOYING.md, g0=kubernetes/tap/DEPLOYING.md, g1=kubernetes/tap/, g2=DEPLOYING.md, g3=DEPLOYING.md, g4=.md} and was rewritten to 'README.md'
┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[1].validated.transformations[0].otherwise.transformations[0].otherwise.transformations[3].apply.transformations[2] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[0].otherwise.transformations[0].otherwise.transformations[4].apply (RewritePath)
┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'kubernetes/tap/.tanzuignore' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=null, folder=kubernetes/tap/, filename=.tanzuignore, g0=kubernetes/tap/.tanzuignore, g1=kubernetes/tap/, g2=.tanzuignore, g3=.tanzuignore, g4=null} and was rewritten to '.tanzuignore'
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[0].otherwise.transformations[1] (UniquePath)
┃ ┃ ┃ ┗ ┗ Debug Multiple representations for path 'README.md', will use the one appearing last 
┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].apply (Merge)
┃ ┃ ┃ ┃  Info Running Merge(ReplaceText, InvokeFragment)
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].apply.sources[0] (ReplaceText)
┃ ┃ ┃ ┃ ┗  Info Will replace [hello-fun->my-serverless-axl]
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].apply.sources[1] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].apply.sources[1].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[1].apply.sources[1].validated.delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].apply.sources[1].validated.delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[1].apply.sources[1].validated.delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#includeBuildToolWrapper) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[1].apply.sources[1].validated.delegate.transformations[0].sources[0].delegate (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [mvnw, mvnw.cmd, .mvn/**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [mvnw, mvnw.cmd, .mvn/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [mvnw, mvnw.cmd, .mvn/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug .mvn/wrapper/maven-wrapper.properties matched [mvnw, mvnw.cmd, .mvn/**] -> included
┃ ┃ ┃ ┗ ┗ ┗ ╺ engine.transformations[1].validated.transformations[1].apply.sources[1].validated.delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2] (Merge)
┃ ┃ ┃ ┃  Info Running Merge(Include, InvokeFragment, InvokeFragment)
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug Tiltfile matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┗ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Let
┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate (Let)
┃ ┃ ┃ ┃ ┃ ┃ Debug Adding symbol workloadJavaVersion with value '21'
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[0].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[0].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[0].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '<java.version>.*<' with '<java.version>21<'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[1].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [build.gradle]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[1].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex 'sourceCompatibility = .*' with 'sourceCompatibility ...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[2].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[2].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [build.gradle.kts]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[2].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '(?<unmodified>JavaVersion\.VERSION_)(\d+)' with '${unmodified}21'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[3].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[3].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/workload.yaml, config/workload-native.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/workload.yaml, config/workload-native.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [config/workload.yaml, config/workload-native.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[3].delegate.transformations[1] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[4].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[4].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/*.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/*.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[4].delegate.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [config/workload*.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug config/workload.yaml matched [config/workload*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[0].sources[4].delegate.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace regex '(?<unmodified>image: bellsoft/liberica-openjdk-\w*:)(\d+)' with '${unmodified}21'
┃ ┃ ┃ ┃ ┗ ┗ ┗ ╺ engine.transformations[1].validated.transformations[2].sources[1].validated.delegate.in.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[2] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[2].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#bsGitRepository != null) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Let
┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.transformations[2].sources[2].validated.delegate (Let)
┃ ┃ ┃ ┃ ┃ ┃ Debug Adding symbol repoUrl with value 'https://github.com?owner=trisberg&repo=my-serverless-axl'
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[2].validated.delegate.in.apply (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(OpenRewriteRecipe, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[1].validated.transformations[2].sources[2].validated.delegate.in.apply.transformations[0] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[2].sources[2].validated.delegate.in.apply.transformations[1] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗ ┗ ┗  Info Will replace regex '(?<beforeBranch>[\s\S]+)(?<branch>branch: [\S]+)(?<rest>[\S\s]*)' with '${beforeBranch}branc...(truncated)'
┃ ┃ ┃ ┏ engine.transformations[1].validated.transformations[3] (UniquePath)
┃ ┃ ┃ ┃ Debug Multiple representations for path 'mvnw', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path '.gitignore', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'mvnw.cmd', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'pom.xml', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'src/test/java/com/example/helloapp/HelloAppApplicationTests.java', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path '.mvn/wrapper/maven-wrapper.properties', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'README.md', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'catalog/catalog-info.yaml', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'src/main/resources/application.properties', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'config/workload.yaml', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'src/main/java/com/example/helloapp/HelloAppApplication.java', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path 'Tiltfile', will use the one appearing last 
┃ ┃ ┃ ┃ Debug Multiple representations for path '.tanzuignore', will use the one appearing last 
┃ ┃ ┃ ┗ Debug Multiple representations for path 'LICENSE', will use the one appearing last 
┃ ┗ ┗ ╺ engine.transformations[1].validated.transformations[4] (Provenance)
┗ ╺ engine.transformations[2] (UniquePath)
```
