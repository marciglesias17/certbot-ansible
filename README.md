# certbot-ansible

Playbook example

```
- hosts: test
  roles: 
    - role: certbot-ansible
      vars: 
        certbot_certificate_domain: "www.example.com"
        certbot_aws_access_key: "test"
        certbot_aws_access_key_id: "0I249mZXzfM2vzqtZiz5+rQ"
        certbot_certificate_method: "aws"
```
