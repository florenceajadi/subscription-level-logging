<h4>Subscription Level Logging</h4>
<p>I'll be tracking activities, security events, and resource health in my subscription. </p>
<p>
  <img src="https://github.com/user-attachments/assets/44fe8ae5-269c-4241-9b3b-35816ad5ace8" height="80%" width="80%" />
</p>
<p>
I was able to create a new diagnostic setting that'll allow me to collect, route, and store logs and metrics from my resources so i'm able to monitor, analyze, and troubleshoot. 
I checked the logs in the category which would allow me to  tracks changes made to resouces like creating or deleting, log security events like access attempts and policy violations
  monitor Azure service status and availability, capture triggered alerts based on set conditions, log optimization suggestions from Azure Advisor, track policy enforcement and compliance checks.
 log actions taken by Azure's autoscale feature, and monitor the health of individual resources.</p>
  <p>
<img src="https://github.com/user-attachments/assets/1558397e-e5e5-412d-bab5-a715c71c8e50" height="80%" width="80%" />
    <img src="" height="80%" width="80%" />
</p>
<p>
I created two resource groups that I will be generating logs from. I will be deleting these two resource groups later.
</p>
<br />
 <p>
<img src="https://github.com/user-attachments/assets/2f69cccc-c49f-4216-a884-c8fbb5f3a772" height="80%" width="80%" />

</p>
<p>
searching for AzureActivity logs for anything related to resource groups that starts with "criticial-infrastructure-", which resulted to 5 resource groups.  It also shows the result by the time
  the activity occurred, which helps me track any operations like deletion on any of the critical resource groups. This is good for monitoring and ensuring the security and integrity of infrastructure.
</p>
<img src="https://github.com/user-attachments/assets/aa0a8488-9654-4996-b2f0-107761306374" height="80%" width="80%" />
<p>
  Using query to filter out the AzureActivity logs to display activities that aren't categorized as 'Administrative' focusing on actions on the management side. Monitoring events like service health updates,
  policy changes, or alerts.
</p>
<br />
<img src="https://github.com/user-attachments/assets/5c037000-027a-4184-b5ed-5be9dc76e5ce" height="80%" width="80%" />
<p>Receiving activites from AzureActivity logs that happened 24hrs ago, which the WRITE filer logs shows only operations involving writing or modifying resources like updates and able to sort the results by the time they were generated, 
  with the most recent first</p>
  
<img src="https://github.com/user-attachments/assets/3a340e5a-8a83-4682-ae6c-150287b3094f" height="80%" width="80%" />
<p>Receiving activities that were successful in the last 30mins from the AzureActivity log and was able to filter operations ending with DELETE and able to sort the most recent activities first.</p>
<br />
<img src="https://github.com/user-attachments/assets/f9609601-82a6-4edb-9bce-abe17974fdd2" height="80%" width="80%" />
<p>activities made to NSGs in Azure speficially on security rules. I was able to filter where security rules within NSGs are modified whether creating, updating, or deleting rules.  
The resource groups </p>
