# Day 1 - Mandi Walls - New Things in Chef #

* Technical Practice Manager @ Chef

* Chef Metal: \m/
    * Policy-based provisioning
    * Use a Chef Server and a "provisioning node" that converges your clusters
    * Can create an image, not leave behind a running machine
* Containers
    * `with_provisioner ChefMetalDocker::DockerProvisioner.new`
    * 1) Create a Docker container host in EC2 with Metal (recipe[docker])
    * 2)
* Enterprise Chef feature: Chef Actions
    * Push Chef actions (converge, create provisioner, etc.) to destinations
    * Send to an analytics platform
    * Send notifications to HipChat


* What if Test Kitchen had a chef-metal driver?
