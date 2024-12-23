# pktFragments

Community project for Autodesk Civil 3D subassemblies.
Feel free to share your PKTs in NET or from Subassembly composer.

- You can easily access it with https://bit.ly/pktfragments
- Repo homepage https://github.com/karfous/pktFragments/tree/main

## What can I find here?

Well, you can navigate to

- [pkt folder](https://github.com/karfous/pktFragments/tree/main/pkt) - here you can download all subassemblies at once
- [subassemblies folder ](https://github.com/karfous/pktFragments/tree/main/subassemblies) - where you can find all the details for each subassembly
- [proCivil folder ](https://github.com/karfous/pktFragments/tree/main/subassemblies/_proCIVIL) - which contains subassemblies from my older project

## HOW TO - collaborate on this repository?

- Fork the repository
- Create new branch
- Describe your subassemblies
- Do a pull request

* how to fork the repository? Well you should know something about github. So you can checkout [1 hour explanation](https://www.youtube.com/watch?v=RGOj5yH7evk), or skip to [how to fork](https://www.youtube.com/watch?v=a_FLqX3vGR4) or other [video explaining usage for a class](https://www.youtube.com/watch?v=3dcZNFwPc6I&ab_channel=BillKerney)

## HOW TO - create README for your subassembly?

Check one of the already released PKTs and copy the structure.

## HOW TO - versioning your subassemblies?

We use [semantic versioning](https://www.linkedin.com/pulse/understanding-semantic-versioning-guide-developers-ajibola-oseni-/) for an output parameters.

Version of a subassembly must be visible for users as an output parameter - create an output parameter in your subassembly an setup its value.

Version: 2018 1.0.7

- 2018 is Subassembly composer version (in you use a composer)
- 1 is first major release
- 0 is first major release
- 7 patching you previous pkts

## HOW TO - naming convention

Name of a subassembly must reflect semantic versioning of a output parameter.

Let´s say we have a Square subassembly from previous example with version 2018 1.0.7. What is the name of the pkt file?

Name of this subassembly would be - Square_2018_1

Why not to use minor anod patch version? Minor and patch versions should NOT break the compatibility. So switching version should be seamless. Only major version can be incompatible with previous release.
