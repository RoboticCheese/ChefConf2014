# Day 1 - Fletcher Nichol - Test Kitchen: The Future #

* Review
    * Declarative static config, aka yaml file
* Coming soon
    * Partial versions, `require_chef_omnibus: 11`

* Hot tips
    * `kitchen list --bare`
    * `kitchen list ubuntu`
    * `kitchen list '^cli-*`
    * `kitchen diagnose`
        * Makes all the implicit stuff explicit
    * Can now configure busser things like root path
    * Chef Zero provisioner - Thank John Keiser
    * `kitchen test --concurrency=3`
* Swapped out parallel for concurrent, celluloid for pure ruby threads
    * Concurrency is not parallelism
    * `kitchen test --concurrency`
* Hyper Dynamic Caching
    * `http_proxy` - Thank AdamJacob
        * Sets env variable honored by wget, curl, etc. etc.
        * Add polipo http cache
* The Future
    * More explicit config
    * Windows - Both as dev system running TK and TK system under test
    * More better test coverage
