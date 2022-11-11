# Cisco SecureX Orchestration Workflows

# Kenna - Create POC Risk Meters

This Cisco SecureX Orchestration workflow creates a set of Kenna Risk Meter groups based on Risk Meter Names and Search Queries stored in the local "Custom RM Table" and a hierarchical RM structure for Windows OS.

Target Group: not required 
Targets: create a Target (HTTP Endpoint) with your API base URL

Steps:
- Select your Target
- Adjust the local Custom RM Table as needed before running this workflow
- Run the workflow 
- Enter required input for workflow execution (API token)
- Workflow is looping through the Custom RM Table
- Creating a new Risk Meter for each row in table with RISKMETERNAME and RISKMETERSEARCH
- Creating hierarchical Risk Meters for all Windows OS 

# Kenna - Generate POC Report

This Cisco SecureX Orchestration workflow collects a set of Kenna vulnerability statistics based on CVSSv2, CVSSv3, Scanner and Kenna Risk scores and sends a report via Email to a list of recipients.

Target Group: not required 
Targets: create a Target (HTTP Endpoint) with your API base URL

Steps:
- Select your Target
- Run the workflow 
- Enter required input for workflow execution (API token, recipients, organization name)
- Workflow collects the data
- Workflow replaces tags in HTTP Email body with data
- Send Email report to recipients

