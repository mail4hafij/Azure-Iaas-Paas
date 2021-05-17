# Azure-Iaas-Paas
The idea here is to setup a multi-tier solution in Azure. The setup is over engineered with the intention to explore possibilities.

## TODO
1. Upload the ARM templates with parameters and veriables.
2. Add a simple WCF project, Node API, and App project.
3. Deploy all three projects.
4. Document the loadBalancer rules (backend pools, health probs, persistancy).
5. Describe the NAT rule for one of the VMs (remote MSSQL connection). This VM contains a MSSQL server, a NODE API project, and a WCF project. THIS IS NOT FOR PRODUCTION SETUP. This is just to show you that, it is possible to share a VM accross different backend pools and even accept inbound connection using NAT. There are couple of steps here (NOT RECOMMENDED FOR PRODUCTION SETUP) - 
    * Install MSSQL server and enable sa account. https://sudeeptaganguly.wordpress.com/2010/04/20/how-to-enable-sa-account-in-sql-server/
    * Enable remote login to the SQL server. https://nishanc.medium.com/how-to-enable-remote-connections-to-sql-server-dc5b6c812b5
    * Create NAT inbound rule for the VM to access remote SQL server ports.
6. Document the setup for Application gateway.
7. Document the setup for Traffic manager (performance based routing).
8. Explain the overall flow.

## Conceptual model
<img src="Architecture.jpg" />
