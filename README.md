Gradle's artifact auto-deployment to Nexus script:

To automate the deployment of artifacts to Nexus using Gradle, you can configure the ```'maven-publish'``` plugin along with the necessary Nexus repository credentials. 
The basic script to achieve this is in ```./build.gradle file```

Replace ```https://your-nexus-url/repository/maven-releases/``` with the URL of your Nexus repository. 
Make sure to replace ```'nexusUsername'``` and ```'nexusPassword'``` with your Nexus credentials. 
You can provide these credentials as Gradle properties or environment variables.

To use this script, you can execute ```./gradlew publishToNexus``` task, it will publish the artifacts to your Nexus repository.