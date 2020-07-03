# Sample Playbooks to Deploy Apps on OpenShift

I created them just to experiment with doing Ansible automation with OpenShift.

I am not an experienced playbooks developer and I am interested in better ways to make my playbooks wait for things to happen and later test that deployment and undeployment are really done so these playbooks are "fire and forget".

I prefer these to be simple and readable than using advanced tricks.
But I am interested in learning tricks that would make these more reusable, flexible, and reliable.

Tested with Ansible 2.9.10 from EPEL under RHEL 8.0 and python3-openshift-0.11.2-1.el8.noarch.

## Hello, World app

* deploy-hello.yaml

This playbook deploys a hello, world app into a new project on OpenShift and tries to access the application.

It assumes you are already logged in to OpenShift and has permission to create new projects (the self-provisioner role).


## Jenkins

* deploy-jenkins.yaml
* undeploy-jenkins.yaml

These playbooks and support files deploy and undeploy Jenkins using the standard template.

These playbooks assume you are alreaddy logged in to OpenShift as a cluster administrator because I am using these templates to deploy a Jenkins instance that I use to apply cluster settings in a tentative GitOps workflow.

They should be easy to adapt to grant Jenkins less permissions, for a typical CI/CD workflow, which would require just developer permissions.

