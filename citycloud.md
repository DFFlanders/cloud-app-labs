If you have any questions about how to use CityCloud contact me on twitter @petterlundkna

# How to use and connect to CityCloud:

clouds.yaml example:

    auth:
      username: osdaust
      password: OS_DaysAust2016!
      tenant_id: 
      project_id: 
      auth_url: https://identity1.citycloud.com:5000/v3/
      user_domain_id: 
    region_name: La1

Sent the passwd and usernames for the control panel and clouds.yaml on hangouts as well buthere you go:

Username: demo20-30 (20,21, 22 and so on)
passwd: OS_DaysAust2016!

https://citycontrolpanel.com is the url for the control panel.
tenant uuids can be found here for an account:

(end of a endpoint url: https://la1.citycloud.com:8776/v2/4bd334da36aa489aaea00daa5b406c57)
also  here: https://citycontrolpanel.com/openstack#manage_projects
user domain id's  will be found here:
https://citycontrolpanel.com/openstack#openstack_api_access

# Previous Instructions:

- Go to https://citycontrolpanel.com, fill in the username and password provided by tweeting and follow @petterlundkna
- You will now see the Dashboard and a Menu on the left side, click API and then Openstack Native API, here you will find your   Openstack Native API user used for shade. You will also find all relevant endpoints and ID’s.
- When creating your clouds.yaml file add 

- the following info:
    - region_name: Lon1
    - auth:
      - username: username
      - password: password
      - tenant_id: found in the endpoint url list “https://lon1.citycloud.com:8776/v2/etc…”
      - project_id: same as Tenant ID
      - auth_url: https://identity1.citycloud.com:5000/v3/
      - user_domain_id:

[Getting started using OpenStack Shade with citycloud](https://www.youtube.com/watch?v=7s7LKdih2vA)
