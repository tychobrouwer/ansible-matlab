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
    matlab_input_file: templates/matlab-input.txt
  
  roles:
    - role: tychobrouwer.matlab

    - role: tychobrouwer.matlab,
      matlab_release: R2024b
      matlab_install_location: /opt/matlab/R2024b
      matlab_working_directory: /home/matlab/Documents
      matlab_user: matlab
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
