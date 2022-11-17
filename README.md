# certbot-ansible

A basic ansible role to deploy SSL certificates with DNS validation, with CloudFlare or AWS.

Everything you need to know to configure the role.

AWS Route53 DNS:
https://certbot-dns-route53.readthedocs.io/en/stable/

CloudFlare DNS:
https://certbot-dns-cloudflare.readthedocs.io/en/stable/


# Requirements

- ansible < 2.13.6


Playbook example.yml
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
