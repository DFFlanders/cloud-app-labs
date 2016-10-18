How to use and connect to CityCloud

- Go to https://citycontrolpanel.com, fill in the username and password provided
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
