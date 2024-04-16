<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<header>
  <h1>Azure NSG and Protocol Inspection Guide</h1>
  <p>This guide details the steps for setting up Network Security Groups and inspecting various network protocols using Wireshark in Microsoft Azure.</p>
</header>

  <h2>Create Resources</h2>
  <ul>
    <li>Create a Resource Group in Azure.</li>
    <li>Create a Windows 10 Virtual Machine and an Ubuntu Virtual Machine within this Resource Group, configuring each with a new Virtual Network (Vnet).</li>
    <li>Review the setup using Network Watcher to ensure all resources are properly connected and configured.</li>
  </ul>
</section>

  <h2>Observe ICMP Traffic</h2>
  <ul>
    <li>Use Remote Desktop to access your Windows VM and install Wireshark.</li>
    <li>Filter Wireshark to display only ICMP traffic and initiate ping requests between your VMs.</li>
    <li>Alter ICMP rules in the Network Security Group to see changes in traffic flow, observing these changes both in Wireshark and through command line outputs.</li>
  </ul>
</section>

  <h2>Observe SSH Traffic</h2>
  <ul>
    <li>Filter for SSH traffic in Wireshark.</li>
    <li>From Windows 10 VM, establish an SSH connection to Ubuntu VM and monitor the SSH traffic.</li>
    <li>Perform commands over SSH and observe how these are captured and displayed in Wireshark.</li>
  </ul>
</section>

  <h2>Observe DHCP Traffic</h2>
  <ul>
    <li>Filter for DHCP traffic in Wireshark.</li>
    <li>Renew IP configuration on your Windows VM to generate DHCP traffic and observe the results in Wireshark.</li>
  </ul>
</section>

  <h2>Observe DNS Traffic</h2>
  <ul>
    <li>Set Wireshark to filter DNS traffic.</li>
    <li>Use nslookup on your Windows VM to query domain names and observe DNS traffic and its details on Wireshark.</li>
  </ul>
</section>

  <h2>Observe RDP Traffic</h2>
  <ul>
    <li>Filter Wireshark for RDP traffic using the specific TCP port.</li>
    <li>Discuss and explain the continuous traffic flow due to the nature of RDP's live stream capabilities.</li>
  </ul>
</section>

  <h2>Lab Cleanup</h2>
  <ul>
    <li>Terminate all sessions and close Wireshark.</li>
    <li>Delete all resources created during the lab exercises to ensure no ongoing charges or security risks.</li>
    <li>Verify that all deletions are complete and resources are fully removed.</li>
  </ul>
</section>

</body>
</html>
