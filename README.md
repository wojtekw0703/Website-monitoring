# Websites monitoring :computer: :cloud:
Simple monitoring for specific websites which presents data about:
- SSL existence and expiry,
- current HTTP code,
- HTTP version,
- Status of a website,
- Traffic
## Main language
- Python :snake:

## Installation

1. Clone the project
```
git clone https://github.com/wojtekw0703/Website-monitoring.git
```
3. Create an account on AWS or make a new account in IAM (copy and keep Account ID :clipboard:) 
4. Configure your machine:
- [node package manager](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm),
- [aws cli](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html),
- [aws cdk](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html),
5. Set credentials for aws default account or specific
6. Update the _.env_ file with proper credentials
7. [Here](https://docs.aws.amazon.com/cdk/v2/guide/hello_world.html) you have the documentation how to run your first AWS CDK app
8. Create a new ```key pair``` on AWS. Connect with EC2 instance via _EC2 Instance Connect_ and update ```~/.ssh/authorized_keys``` to be able to connect with EC2 from e.g Putty, MobaXterm.
In case of troubles with permissions, run ```$ chmod 600 ~/.ssh/authorized_keys```
8. Install Ansible locally
9. Install all dependencies
10. Run ```ansible-playbook --connection=local  monitoring.yml``` to make it locally
11. Remember about editing _Security groups_ and _Inbound rules, Outbound rules_ to be able see Grafana & Prometheus sites

## Screenshots
![Capture](https://user-images.githubusercontent.com/33324211/172939398-b2899c99-6d37-49e6-9e18-e8495557ee5f.PNG)
![Capt2ure](https://user-images.githubusercontent.com/33324211/172939404-d5af9439-96ac-411c-8b99-a51d585a97cc.PNG)

