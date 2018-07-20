# F5_Big-IP_LTM_examples
F5 Big-IP load balancing examples

The dynamic_pool_patching.yml is utilized for dynamic patching of pool members with minimal information required from the end user. This example is made for use with tower using custom credentials but please note credentials can be passed in each task as noted in the commented out fields.

dynamic_pool_patching.yml needs to have the following variables provided:

lb_server: "192.168.1.89" - This is the load balancer you are targeting.
poolserver: "webservers" - This is the pool you are targeting for patching.

If you are using ansible-engine and not tower you will need to pass the credentials via the commented out strings for user: ans password to the F5 Load Balancer on the F5 tasks. These credentials can ofcourse be variableized and then pushed from Ansible Vault. 
