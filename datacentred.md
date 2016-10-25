# Using DataCentred for Cloud App Labs

If you need a username, password and project name please [get in touch with @code_sean](http://ctt.ec/gZa51)

## Dashboard Access

You can access our user dashboard via https://my.datacentred.io

You can access the Horizon dashboard via: https://compute.datacentred.io

## Via API

Our Keystone service is available via https://compute.datacentred.io:5000/v2.0/. The service catalog contains details for other API endpoints supported.

## Using clouds.yaml

If you're using a clouds.yaml file, populate the information within it using your credentials like so:

```yaml
# clouds.yaml

clouds:
  datacentred:
    auth:
      username: test_account_1@openstacksummit.org
      password: Password123
      project_name: barcelona_summit_1
      auth_url: https://compute.datacentred.io:5000/v3
      domain_name: default
```

```python
# shade_test.py

import shade
cloud = shade.openstack_cloud(cloud='datacentred')
image  = cloud.get_image('ef24441d-01ad-4006-b63d-6da67b7f1348')
```

## Video Demo with Shade

[![Getting started with shade on datacentred](http://img.youtube.com/vi/pwq0_FQIAHk/0.jpg)](http://www.youtube.com/watch?v=pwq0_FQIAHk)
