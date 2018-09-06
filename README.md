# Preflight-checks Automation
<h3> Introduction </h3>
<p>As we all know that pre-flight check is very time-consuming process and every time a minty upgrade batch comes it takes a lot of time of SRE to manually perform the pre-flight checks and format the output of each check. To resolve this issue, I have created a bash script to automate all the checks for pre-flight checks as well as to format the output of all the checks as per JIRA format.

After running following script SRE will just need to verify the output and copy and paste the output directly in JIRA as it will be pre-formatted :wink:

preflightChecks_minty script provides the output of following checks:
<ol type="1">
  <li>Smoke Test</li>
  <li>Disk Space</li>
  <li>Current Splunk Version</li>
  <li>Splunk is running as Splunk User status</li>
  <li>Admin password status</li>
  <li>Premium Apps status</li>
  <li>EBS Attachment</li>
  <li>Stack HEC Status</li>
  <li>Cluster-Status</li>
  <li>Stack Overview</li>
</ol>

<strong>NOTE:</strong> Checks<strong> 7</strong> to<strong> 10</strong> are provided in form of URL links which you can open using<strong> COMMAND + Double Tap</strong>.
</p>
<h3> Setup </h3>
<ol>
  <li>Clone the preflightChecks_minty file into <b>Tower</b></li>
  <li>Give that file executable permissions</li>
  <code> chmod +x preflightChecks_minty</code>
</ol>
<Strong>Don't refresh stack before executing preflightChecks_minty as it will refresh the stack on it'w own;)<strong>
<p>
<h3> Usage: </h3> 
  <code> ./preflightChecks_minty -s StackName</code>
</p>

![preflight_output](https://user-images.githubusercontent.com/39366638/45172782-fa6f5580-b223-11e8-8999-ba0b1b5d7f16.gif)

<p>
<strong>Important Notes:</strong> 
<ol>
<li>As of now this script will only work in Tower directory
<li>Please verify all the output before pasting in JIRA. This is just a script, it's not as smart as us :wink:
 </ol>
Problems/Suggestions? Feel free to open an issue/PR! </p>
