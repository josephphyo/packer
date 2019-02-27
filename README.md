# My Packer Template


![](/packer.png)


> My Packer Template for Build Automated Machine Images.
## What is Packer? 
    
>> Packer is an open source tool for creating identical machine images for multiple platforms from a single source configuration. Packer is lightweight, runs on every major operating system, and is highly performant, creating machine images for multiple platforms in parallel. Packer does not replace configuration management like Chef or Puppet. In fact, when building images, Packer is able to use tools like Chef or Puppet to install software onto the image. A machine image is a single static unit that contains a pre-configured operating system and installed software which is used to quickly create new running machines. Machine image formats change for each platform. Some examples include AMIs for EC2, VMDK/VMX files for VMware, OVF exports for VirtualBox, etc.
## Packer Terminology

>>**Builds** are a single task that eventually produces an image for a single platform. Multiple builds run in parallel. Example usage in a sentence: "The Packer build produced an AMI to run our web application." Or: "Packer is running the builds now for VMware, AWS and VirtualBox." <br />
>>**Provisioners** are components of Packer that install and configure software within a running machine prior to that machine being turned into a static image. They perform the major work of making the image contain useful software. Example provisioners include shell scripts, Chef, Puppet, etc. <br />
>>**Templates** are JSON files which define one or more builds by configuring the various components of Packer. Packer is able to read a template and use that information to create multiple machine images in parallel.

### Usage 

- Install Packer on your own Machine.
    >>>> **URL: [Packer Docs](https://www.packer.io/docs/install/index.html)**

- Put Access Key and Secret Key From AWS.
    >>>> **Strongly Recommend to use IAM User instead of Root User**

- Change Permisson for Provision Scripts.
    >>>> $ chmod +x provision.sh

- Validate Packer Templates. 
    >>>> ***$ packer validate*** example.json
           **Result** Template validated successfully.

- Run/Build Packer Template.
    >>>> ***$ packer build*** example.json

Reference: **URL: [https://www.packer.io/docs/index.html](https://www.packer.io/docs/index.html)**

---


