Influx
=========

Install [Shairport Sync](https://github.com/mikebrady/shairport-sync) for a Raspberry Pi.  Tested on Rasbian Stretch.

Requirements
------------

Tested on Rasbian Stretch

Role Variables
--------------
* `shairport_sync_repo` - Location of Shaiport Sync Git repository (default: https://github.com/mikebrady/shairport-sync.git )
* `shairport_sync_version` - Version to checkout (default: 3.1.3)
* `shairport_sync_name` - Advertized name of the Shairport Sync service (default: Test Shairport Sync Server)
* `shairport_sync_output_device` - Output device to play to (default: default)
* `shairport_sync_mixer_control_name` - Name of the mixer to use (default: PCM)


Dependencies
------------

None


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
    - hosts: servers
      roles:
         - { role: kfieldho. }
         - { role: kfieldho.shairport-sync, shairport_sync_name: "Living Room Speakers", shairport_sync_output_device: "hw:1", shairport_sync_mixer_control_name: "Speaker" }
```

Note: Role example configures Rasberry Pi with Sabrent USB sound "card"

License
-------

BSD

Author Information
------------------

Keith Fieldhouse
@kfieldho on GitHub
github@fieldhouses.net
