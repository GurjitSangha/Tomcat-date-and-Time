node {
   // Mark the code checkout 'stage'....
   stage 'Checkout'

   // Get some code from a GitHub repository
   git url: 'https://github.com/GurjitSangha/Tomcat-date-and-Time'

   // Get the maven tool.
   // ** NOTE: This 'M3' maven tool must be configured
   // **       in the global configuration.           
   def mvnHome = tool 'm3'

   // Mark the code build 'stage'....
   stage 'Build'
   // Run the maven build
   sh "cd SimpleMavenWebapp && mvn package"
}
