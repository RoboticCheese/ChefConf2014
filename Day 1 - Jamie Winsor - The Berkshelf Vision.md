# Day 1 - Jamie Winsor - The Berkshelf Vision #

* What Do I Do With My Hands and Why is My Posture So Bad?
* Lead Platform Engineer, Undead Labs
    * State of Decay
* Berkshelf 3.0 is out
    * 150x resolver speed improvement
    * Uses Chef's cookbook resolver, more accurate
    * Part of the Chef DK
* Berkshelf core team: Jamie, Seth Vargo, Michael Ivey
* Three requirements for any self-contained release:
    * Software artifact
    * Cookbook artifact
        * Resides in same repo as software
        * Should share version of software artifact
        * Build with `cd cookbook && berks package`
        * See https://github.com/berkshelf/berkshelf-api
            * Uses GitHub cookbook to pull in release from GiHub via LWRP
                * `github_asset` resource
            * Provides resource for extracting that GH tarball
                * `libarchive_file` resource
    * Install/upgrade instructions
* Why should the cookbook live with the software?
    * Brings teams together
* Berkshelf now compiles metadata on vendoring or uploading
    * No more errors from `long_description File.open()`
* Release artifacts to GitHub with Octokit and a rake task
    * (See also Stove)
* Also recently released berkflow: cookbook-centric deployment workflow tool
    * Install to the Chef DK w/ `sudo blo gem install blah`
    * `blo install https://github.com/berkshelf/...`
    * `blo upgrade berks-api-dev berkshelf-api 1.2.1`
    * Or `blo up` but not `blo me`
* Also Undead Labs is hiring
