# Day 2 - John Keiser - Chef Metal Update #

* Ye olde ops playbook: Evil
* Ye not so olde ops playbooks: `knife ec2 ... ... ...` still kind of evil
* "How do I version/test/scale my cluster?"
    * "The same way I do a server already!"
* `machine` resource + provisioners = Metal!
* Commands:
    * `metal login`
    * `metal execute`
    * ...
* Four machine actions: create, delete, get, stop
* Already supports Windows transport via WinRMTransport
    * Also SSH, LXC, Docker
* `server.running?`
* Different machines can be behind different provisioners
* `with_provisioner` block: everything after this will use that prov.
* `with_provisioner` attribute of a machine - just that machine
* Can also point different machines at different Chef servers
* The future
    * Parallelism (when it comes to Chef itself)
    * More provisioners: Xen, Razor, Crowbar, etc.
    * ***Eventually merge Metal into Chef itself***
