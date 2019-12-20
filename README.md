Packer-Templates-Vyos
=====================

Packer templates to create VyOS build images.

Forked from a project by Yuya Kusakabe (higebu), and updated for the latest
VyOS development (rolling version) of VyOS (vyos 1.3-rolling).

All earlier versions have not been touched.

Artefact outputs (build images) are in the form of Vagrant box files.
Using the post-processor options within the template (keep_input_artifact=true),
  artefacts (VM files) can be retained to run up VMs outside of Vagrant.

Notes:
Development and not for production use.
Bug reported in VyOS (http://phabricator.vyos.net/T1880) causes long hang time on
  reboot. Wait time increased within the template to over 200s to compensate,
  therefore image creation takes longer that it would otherwise.
