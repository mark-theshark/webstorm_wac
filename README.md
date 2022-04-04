# JetBrains WebStorm IDE and HelloWorld Node.js and React app (coder-react)

###### Instructions

1. Open the git provider toggle for embeddable buttons for each Coder deployment (Kubernetes cluster where Coder is installed)
1. Choose either a template or an image to build a workspace based on the image, compute and configuration settings


<details>
  <summary>More Info</summary>

[Workspace templates](https://coder.com/docs/coder/latest/workspaces/workspace-templates) are declarative YAML files that describe
how to configure Coder workspaces and their supporting infrastructure. Coder supports
files with either the `.yaml` or `.yml` extension.

[Images](https://coder.com/docs/coder/latest/workspaces/images) contain the IDEs, CLIs, language versions, and dependencies users need to work on software development projects. Users can create workspaces with the image as the blueprint, then begin contributing immediately to the projects for which the image was defined. Images may contain [configure scripts](https://coder.com/docs/coder/latest/images/configure) that Coder runs after the workspace build to add additional dependencies, VS Code extensions, clone repositories, or run CLI commands.

> Both templates and images require that OAuth has been configured on the git provider and the Coder user has linked their Coder account to the git provider (copies their Coder-generated SSH public key) for git clone, push and pull actions.
</details>

> A Coder workspace is an isolated pod and inner container managed by the Coder control plane running in a namespace of a Kubernetes cluster. The Coder deployments below are running on GCP GKE.

##### from image

###### clean.demo.coder.com
[![Open in Coder](https://clean.demo.coder.com/static/image/embed-button.svg)](https://clean.demo.coder.com/workspaces/git?org=624ad5c6-12323dfa5f76cb23f9238d15&image=624ad7ed-15da9151456f625244237b15&tag=ubuntu&service=github&repo=git@github.com:mtm20176/webstorm_wac.git)

##### from template

###### clean.demo.coder.com
[![Open in Coder](https://cdn.coder.com/embed-button.svg)](https://clean.demo.coder.com/wac/build?template_oauth_service=github&template_url=git@github.com:mtm20176/webstorm_wac.git&template_ref=main&template_filepath=.coder/coder.yaml)













