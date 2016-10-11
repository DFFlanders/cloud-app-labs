# Using Internap for Cloud App Labs

You should've been given an API username (in the form of api-XXXXXXXXXXX), password and tenantID (in the form of inap-XXXXX).

## Horizon access

You can access your horizon dashboard via https://horizon.internap.com.
Ensure to always select to the right region (see the step 2 of the horizon walkthrough below) : there is 6 regions available, but free account are restricted to
 * ams01 (Amsterdam)
 * nyj01 (New Jersey)

## API access

Keystone is available via https://identity.api.cloud.iweb.com/v2.0 or https://identity.api.cloud.iweb.com/v3 (depending of which version of Keystone you want to use).
The service catalog contains details for other API endpoints supported and your tenant UUID.

The other service are available at :
Compute/Nova - https://compute.api.nyj01.cloud.iweb.com/v2/<your-tenant-UUID>
Image/Glance - https://image.api.nyj01.cloud.iweb.com
Volume/Cinder - https://volume.api.nyj01.cloud.iweb.com/v2/<your-tenant-UUID>
ObjectStore/Swift - https://object-store.api.nyj01.cloud.iweb.com/v1/AUTH_<your-tenant-UUID>
Heat/Orchestration - https://orchestration.api.nyj01.cloud.iweb.com/v1/<your-tenant-UUID>
AWS Cloudformation compatibility - https://cloudformation.api.nyj01.cloud.iweb.com/v1

## Simple example using clouds.yaml

If you're using a clouds.yaml file, populate the information within it using your credentials like so:

```yaml
# clouds.yaml

clouds:
  internapNYJ:
    profile: internap
    auth:
      username: api-XXXXXXXXXXXX
      password: <your-password>
      project_name: <your-tenant-ID>
      region_name: nyj01
  internapAMS:
    profile: internap
    auth:
      username: api-XXXXXXXXXXXX
      password: <your-password>
      project_name: <your-tenant-ID>
      region_name: ams01
```

```python
# list_images.py
from shade import *

simple_logging(debug=True)
conn = openstack_cloud(cloud='internapNYJ')

print( 'Listing images' )
images = conn.list_images()
for image in images:
	print( '--> image details :'+ image["name"] + ' - ID : ' + image["id"] )

print( 'Done! Congrats' )
```

## Horizon walkthrough
1. Login to https://horizon.internap.com ![walkthrough - step 1](/img/inap-horizonwalk-1.png)
2. Select the *AMS01* region ![walkthrough - step 2](/img/inap-horizonwalk-2.png)
3. Select the Instances tab and click on ‘Launch an Instance’. Fill up the Instance Name, select ‘Boot from image’ for your Instance Boot Source and your preferred OS in Image Name. ![walkthrough - step 3](/img/inap-horizonwalk-3.png)
4. In the ‘Access & Security’ tab, choose an admin password and confirm (or select a SSH keypair) ![walkthrough - step 4](/img/inap-horizonwalk-4.png)
5. In the ‘Networking’ tab, select the network you want activate -LAN or WAN- If you use both, make sure to drag-and-drop the network with ‘WAN’ in his name first![walkthrough - step 5](/img/inap-horizonwalk-5.png)
6. *Always* put WAN first! ![walkthrough - step 6](/img/inap-horizonwalk-6.png)
7. Click launch! you’re done! ![walkthrough - step 7](/img/inap-horizonwalk-7.png)

## Video Demo with Shade

[![Internap Shade demo Part Deux ("Two" but David is funny!)](https://www.youtube.com/watch?v=JyQHoDoypGM](https://www.youtube.com/watch?v=JyQHoDoypGM)
