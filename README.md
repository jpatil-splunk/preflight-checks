# Preflight-checks Automation
<h3> Introduction </h3>
<p>As we all know that pre-flight check is very time-consuming process and every time a minty upgrade batch comes it takes a lot of time of SRE to manually perform the pre-flight checks and format the output of each check. To resolve this issue, I have created a bash script to automate all the checks for pre-flight checks as well as to format the output of all the checks as per JIRA format.

After running following script SRE will just need to verify the output and copy and paste the output directly in JIRA as it will be pre-formatted ;) </p>

<h3> Setup </h3>
<ol>
  <li>Clone the preflightChecks_minty file into <b>Tower</b></li>
  <li>Give that file executable permissions</li>
  <code> chmod +x preflightChecks_minty</code>
</ol>
  
<p>
<h3> Usage: </h3> 
  <code> ./preflightCheck_minty -s StackName</code>
</p>

![preflight_output](https://user-images.githubusercontent.com/39366638/45172782-fa6f5580-b223-11e8-8999-ba0b1b5d7f16.gif)
