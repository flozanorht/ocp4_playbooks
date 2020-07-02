# Sample Playbooks to Deploy Jenkins on OpenShift

These playbooks and support files deploy and undeploy Jenkins using the standard template.

I created them just to experiment with doing Ansible automation with OpenShift.

All playbooks assume you are alreaddy logged in to OpenShift as a cluster administrator because I am using these templates to deploy a Jenkins instance that I use to apply cluster settings in a tentative GitOps workflow.
They should be easy to adapt to grant Jenkins less permissions, for a typical CI/CD workflow, and require just developer permissions.

I am not an experienced playbooks developer and I am interested in better ways to make my playbooks wait for things to happen and later test that deployment and undeployment are really done so these playbooks are "fire and forget".

I prefer these to be simple and readable than using advanced tricks.
But I am interested in learning tricks that would make these more reusable, flexible, and reliable.
