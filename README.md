Install and configure MATLAB
=========

The role installs and configures MATLAB.

Role Variables
--------------

Example Playbook
----------------

```yaml
    - hosts: servers
      vars:
        password: "password123"
      
      roles:
         - { role: tychobrouwer.matlab,
             matlab_input_file: templates/matlab-input.txt }
         - { role: tychobrouwer.matlab,
             matlab_input_file: templates/matlab-input.txt,
             matlab_install_location: "/opt/matlab/{{ matlab_release }}",
             matlab_user: "matlab"
           }
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
