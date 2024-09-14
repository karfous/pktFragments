# pktFragments

Community project for Autodesk Civil 3D subassemblies.
Feel free to share your PKTs in NET or from Subassembly composer.

## What can I find here?

Well, you can navigate to ...
... pkt folder where you can download all subassemblies at once
... subassemblies folder where you can find all the details for each subassembly

## HOW TO - collaborate on this repository?

Fork the repository
Create your subassemblies
Create a pull request

## HOW TO - create README for your subassembly?

Check one of the already released PKTs and copy the structure.

## HOW TO - versioning your subassemblies?

We use semantic versioning for an output parameters - see https://www.linkedin.com/pulse/understanding-semantic-versioning-guide-developers-ajibola-oseni-/

Version of a subassembly must be visible for users as an output parameter - create an output parameter in your subassembly an setup its value.

Version: 2018 1.0.7
2018 is Subassembly composer version (in you use a composer)
1 is first major release
0 is first major release
7 patching you previous pkts

## HOW TO - naming convention

Name of a subassembly must reflect semantic versioning of a output parameter.

Let´s say we have a Square subassembly from previous example with version 2018 1.0.7. What is the name of the pkt file?

Name of this subassembly would be - Square_2018_1

Why not to use minor anod patch version? Minor and patch versions should NOT break the compatibility. So switching version should be seamless. Only major version can be incompatible with previous release.
