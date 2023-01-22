example of backup Jenkins files. </br>
**Jenkins Job/Pipeline:** </br>
Backup all critical files  -> </br>
Archive files (zip), if needed -> </br>
Transfer to GitHub repo </br>
*credentials.xml* will be stored in AWS S3 after deployment </br>
Plugins: </br>
• [ThinBackup](https://plugins.jenkins.io/thinBackup/) </br>
• [HTTP Request](https://www.jenkins.io/doc/pipeline/steps/http_request/) </br>
  </br>  
**Terraform:** </br>
Create a new ec2 instance with jenkins </br>
Bash script: </br>
Install </br>
• Java SDK 11 </br>
• Docker </br>
• Jenkins </br>
• Jenkins CLI </br>
• Unzip utility </br>
Download files from the repo: https://github.com/kapalulz/jenkins_gitPush_addon/archive/refs/heads/main.zip </br>
Unzip into the jenkins folder </br>
Delete downloaded files. </br>
