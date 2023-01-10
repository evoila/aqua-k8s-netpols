This script is provided as a YAML file. 

Please note before that some configurations still need to be adjusted as this policy set is written in general. 

The rules are based on the Aqua Network Connectivity Requirements (Ports) and can be 

Retrieved from this link: [https://docs.aquasec.com/v2022.4/platform/aqua-environment-and-configuration/network-connectivity-requirements-ports/] 

The policies were configured with egress traffic to Kubernetes DNS to resolve DNS requests. 

In addition, these rules are created for the default Namespace (you can customize this of course). 

the incoming, as well as the outgoing traffic is controlled by Pod selector. In this case the 

Aqua components were labeled and referenced in the policy. So it is a prerequisite that the respective Aqua components are labeled, for example in our file they were labeled as follows --> Aqua Gateway is labeld as app: aqua-gateway etc. But you can customize them as you like, as long as the labels are mentioned correctly in the policies. 

Also note the comments that are included in the script. 

 

