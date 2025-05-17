<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Azure VM Setup for Small Business IT</title>
</head>
<body>

<p align="center">
  <img src="https://i.imgur.com/4wqxHID.png" alt="Microsoft Azure Logo" width="60%">
</p>

<h1>Azure Virtual Machine Setup for Small Business IT</h1>
<p>This project demonstrates how a small business—like a dental clinic or startup—can deploy a cloud-based IT environment using Microsoft Azure. You'll learn how to spin up a virtual machine to support remote access, centralized resources, and secure admin controls.</p>

<h2>Use Case</h2>
<p>A 10-person dental office is opening a second location and needs access to its scheduling and billing software. Instead of buying new physical servers, the office deploys a Windows virtual machine using Azure to enable remote access for all staff.</p>

<h2>Key Features</h2>
<ul>
  <li>Fully cloud-based deployment using Microsoft Azure</li>
  <li>Secure, RDP-enabled access for remote staff</li>
  <li>Scalable setup for file storage, application hosting, or Active Directory</li>
  <li>Step-by-step screenshots included</li>
</ul>

<h2>Requirements</h2>
<ul>
  <li>Computer with internet connection</li>
  <li>Microsoft account</li>
  <li>Credit card (required for Azure’s free $200 credit)</li>
</ul>

<h2>Configuration Steps</h2>

<h3>Step 1: Create an Azure Account</h3>
<p><a href="https://azure.microsoft.com/en-us/free/">Sign up here</a> and claim your free credit.</p>
<ol>
  <li>Click <strong>Start Free</strong></li>
  <li>Enter your info and verify with a credit card (you won’t be charged)</li>
  <li>Access the portal at <a href="https://portal.azure.com">portal.azure.com</a></li>
</ol>
<p align="center">
  <img src="https://i.imgur.com/4wqxHID.png" alt="Microsoft Azure Logo" width="60%">
</p>

<h3>Step 2: Create a Resource Group</h3>
<ul>
  <li>Search <strong>“Resource group”</strong> and select <strong>Create</strong></li>
  <li>Name it (e.g., <code>RG-Lab-1</code>) and choose a region (e.g., <code>West US 3</code>)</li>
  <li>Click <strong>Review + Create</strong></li>
</ul>
<p><img src="https://i.imgur.com/Afnk87u.png" alt="Create Resource Group" width="80%"></p>
<p align="center">
  <img src="https://i.imgur.com/4wqxHID.png" alt="Microsoft Azure Logo" width="60%">
</p>

<h3>Step 3: Create a Storage Account</h3>
<ul>
  <li>Search <strong>“Storage Account”</strong> and click <strong>Create</strong></li>
  <li>Use the same resource group and region</li>
  <li>Name it something like <code>rglab1</code></li>
  <li>Click <strong>Review + Create</strong></li>
</ul>
<p><img src="https://i.imgur.com/zhb3GHZ.png" alt="Create Storage Account" width="80%"></p>
<p align="center">
  <img src="https://i.imgur.com/4wqxHID.png" alt="Microsoft Azure Logo" width="60%">
</p>

<h3>Step 4: Create a Virtual Machine</h3>
<ul>
  <li>Search <strong>“Virtual Machine”</strong> and select <strong>Create</strong></li>
  <li>Use the same resource group and region</li>
  <li>Choose:</li>
  <ul>
    <li><strong>Name</strong>: <code>VirtualMachine</code></li>
    <li><strong>Image</strong>: Windows 10 Pro</li>
    <li><strong>Size</strong>: Standard D2as_v4</li>
    <li><strong>Username</strong>: <code>labuser</code></li>
    <li><strong>Password</strong>: (your chosen password)</li>
  </ul>
  <li>Accept licensing terms and click <strong>Review + Create</strong></li>
</ul>
<p><img src="https://i.imgur.com/p9UJXND.png" alt="VM Setup" width="80%"></p>
<p align="center">
  <img src="https://i.imgur.com/4wqxHID.png" alt="Microsoft Azure Logo" width="60%">
</p>

<h3>Step 5: Connect to the VM</h3>
<h4>Windows:</h4>
<ul>
  <li>Open <strong>Remote Desktop</strong></li>
  <li>Enter the <strong>public IP</strong> from your Azure portal</li>
  <li>Log in with your username/password</li>
</ul>

<h4>Mac:</h4>
<ul>
  <li>Download <strong>Microsoft Remote Desktop</strong> from the App Store</li>
  <li>Click <strong>Add PC</strong>, paste in the IP</li>
  <li>Log in and connect</li>
</ul>
<p><img src="https://i.imgur.com/T4Oc2RX.png" alt="RDP Login" width="80%"></p>
<p align="center">
  <img src="https://i.imgur.com/rEBpL8Y.png" alt="Azure Portal" width="70%">
</p>

<h2>Cleanup Tip</h2>
<p>Delete your resource group after the lab to avoid charges:</p>
<ul>
  <li>Go to <strong>Resource Groups</strong></li>
  <li>Click <strong>Delete</strong> to remove all associated resources</li>
</ul>

<h2>Bonus</h2>
<p>Want to build a ticketing system on your new VM?<br>
Check out <a href="https://github.com/RoslyndWilliams/osTicket--Prerequisites-and-Installation">Part 1 of my osTicket lab</a></p>

<p><em>Created by Roslynd Williams – bridging tech fluency with customer-centered sales insight.</em></p>

</body>
</html>
