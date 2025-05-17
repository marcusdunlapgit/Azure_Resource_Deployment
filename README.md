<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
</head>
<body>

<p align="center">
  <img src="https://i.imgur.com/4wqxHID.png" alt="Microsoft Azure Logo" width="60%">
</p>

<h1>Azure Virtual Machine Deployment for Growing Organizations</h1>
<p>This project demonstrates how a growing organization—such as a dental clinic or startup—can deploy a secure, scalable cloud-based IT environment using Microsoft Azure. The goal is to enable centralized resource management, remote access, and administrative control without the need for physical hardware.</p>

<h2>Business Use Case</h2>
<p>An expanding dental office is opening a new location and needs shared access to scheduling and billing applications. Instead of investing in physical infrastructure, the business leverages Azure virtual machines to allow secure, remote access to all authorized personnel.</p>

<h2>Key Features</h2>
<ul>
  <li>100% cloud-based solution utilizing Microsoft Azure infrastructure</li>
  <li>Secure, RDP-enabled virtual machine access for remote staff</li>
  <li>Flexible architecture suitable for application hosting, file storage, or Active Directory integration</li>
  <li>Step-by-step configuration with visual references</li>
</ul>

<h2>Requirements</h2>
<ul>
  <li>Computer with an active internet connection</li>
  <li>Microsoft account</li>
  <li>Credit card (required to activate Azure’s free $200 credit)</li>
</ul>

<h2>Configuration Steps</h2>

<h3>Step 1: Create an Azure Account</h3>
<p><a href="https://azure.microsoft.com/en-us/free/">Sign up here</a> and claim your free credit.</p>
<ol>
  <li>Click <strong>Start Free</strong></li>
  <li>Enter your information and verify with a credit card (no charges will be made)</li>
  <li>Log in to the Azure portal at <a href="https://portal.azure.com">portal.azure.com</a></li>
</ol>
<p align="center">
  <img src="https://i.imgur.com/4wqxHID.png" alt="Microsoft Azure Logo" width="60%">
</p>

<h3>Step 2: Create a Resource Group</h3>
<ul>
  <li>In the search bar, type <strong>“Resource group”</strong> and click <strong>Create</strong></li>
  <li>Assign a name (e.g., <code>RG-Organization</code>) and choose a suitable region (e.g., <code>West US 3</code>)</li>
  <li>Click <strong>Review + Create</strong> to proceed</li>
</ul>
<p><img src="https://i.imgur.com/Afnk87u.png" alt="Create Resource Group" width="80%"></p>
<p align="center">
  <img src="https://i.imgur.com/4wqxHID.png" alt="Microsoft Azure Logo" width="60%">
</p>

<h3>Step 3: Create a Storage Account</h3>
<ul>
  <li>Search for <strong>“Storage Account”</strong> and click <strong>Create</strong></li>
  <li>Use the same resource group and region you selected earlier</li>
  <li>Assign a unique name (e.g., <code>orgstorage01</code>)</li>
  <li>Click <strong>Review + Create</strong></li>
</ul>
<p><img src="https://i.imgur.com/zhb3GHZ.png" alt="Create Storage Account" width="80%"></p>
<p align="center">
  <img src="https://i.imgur.com/4wqxHID.png" alt="Microsoft Azure Logo" width="60%">
</p>

<h3>Step 4: Deploy a Virtual Machine</h3>
<ul>
  <li>Search for <strong>“Virtual Machine”</strong> and select <strong>Create</strong></li>
  <li>Configure as follows:</li>
  <ul>
    <li><strong>Name</strong>: <code>OrgVM</code></li>
    <li><strong>Image</strong>: Windows 10 Pro</li>
    <li><strong>Size</strong>: Standard D2as_v4</li>
    <li><strong>Username</strong>: <code>labuser</code></li>
    <li><strong>Password</strong>: your secure password</li>
  </ul>
  <li>Accept licensing terms and click <strong>Review + Create</strong></li>
</ul>
<p><img src="https://i.imgur.com/p9UJXND.png" alt="VM Setup" width="80%"></p>
<p align="center">
  <img src="https://i.imgur.com/4wqxHID.png" alt="Microsoft Azure Logo" width="60%">
</p>

<h3>Step 5: Connect to the Virtual Machine</h3>

<h4>Windows:</h4>
<ul>
  <li>Open <strong>Remote Desktop Connection</strong></li>
  <li>Enter the VM’s <strong>public IP address</strong></li>
  <li>Log in using the credentials you created</li>
</ul>

<h4>Mac:</h4>
<ul>
  <li>Download <strong>Microsoft Remote Desktop</strong> from the App Store</li>
  <li>Add a new PC using the VM's public IP</li>
  <li>Log in to establish your remote session</li>
</ul>
<p><img src="https://i.imgur.com/T4Oc2RX.png" alt="RDP Login" width="80%"></p>
<p align="center">
  <img src="https://i.imgur.com/rEBpL8Y.png" alt="Azure Portal Screenshot" width="70%">
</p>

<h2>Cost Management and Cleanup</h2>
<p>To prevent unnecessary charges after completing the setup:</p>
<ul>
  <li>Navigate to <strong>Resource Groups</strong> in the Azure portal</li>
  <li>Select the resource group you created</li>
  <li>Click <strong>Delete</strong> to remove all associated components</li>
</ul>

<h2>Optional Extension</h2>
<p>Interested in deploying a ticketing system on your Azure VM?<br>
Check out <a href="https://github.com/RoslyndWilliams/osTicket--Prerequisites-and-Installation" target="_blank">Part 1 of the osTicket lab guide</a>.</p>

<p><em>Created by Marcus Dunlap – combining technical fluency with a customer-first mindset.</em></p>

</body>
</html>
