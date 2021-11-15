# Fedora-Contributions
A list of all fedora Contributions that I have made

- I added Code of conduct link to footer of each page on fedora-docs and fixed this [issue](https://pagure.io/fedora-docs/docs-fp-o/issue/132). 

  Contribution URL- https://pagure.io/fedora-docs/fedora-docs-ui/pull-request/12
  
- Many people were confused that the local preview of this repository should look like the actual fedora site as discussed in 
  [this](https://pagure.io/fedora-docs/fedora-docs-ui/issue/29) issue. They need to be informed that the local preview of this repository will build only the UI of the project.   The actual fedora site is build using the   [builder repository](https://pagure.io/fedora-docs/docs-fp-o). So I added a note in README which will clarify this point to those   who try to setup this repository. Since this   repository currently needs node version 10 and gulp version 3, so I mentioned this point also in README file.

  Contribution URL- https://pagure.io/fedora-docs/fedora-docs-ui/pull-request/42
  
- The container image for this repository is not updated. To figure out the problem I created a container from this image using podman. There I founded that pre installed node   version is 12 in this image due to which it is giving Assertion error. When I downgraded the node version to 10, it runs successfully. Thus the image needs to be modified as   builder script is using this image to build this repository. So I created an issue an fedora-docs-ui

  Contribution URL- https://pagure.io/fedora-docs/fedora-docs-ui/issue/44
  
- Some commands in antora-ui-builder script is wrong due to which it is not giving the desired results. So I changed the commands which fixed this issue. I also changed the       commands in README file which were wrongly mentioned. This will help people who want to setup this repository using script.

  Contribute URL: https://pagure.io/fedora-docs/fedora-docs-ui/pull-request/45
