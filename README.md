<!-- Header block for project -->
<hr>

<div align="center">

![logo](https://user-images.githubusercontent.com/3129134/163255685-857aa780-880f-4c09-b08c-4b53bf4af54d.png)

<h1 align="center">Unity Helm Repository</h1>
<!-- ☝️ Replace with your repo name ☝️ -->

</div>

<pre align="center">This repository allows for deployment of Helm charts to the Unity Kubernetes Cluster.</pre>
<!-- ☝️ Replace with a single sentence describing the purpose of your repo / proj ☝️ -->

<!-- Header block for project -->

[INSERT YOUR BADGES HERE (SEE: https://shields.io)] [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)
<!-- ☝️ Add badges via: https://shields.io e.g. ![](https://img.shields.io/github/your_chosen_action/your_org/your_repo) ☝️ -->

[INSERT SCREENSHOT OF YOUR SOFTWARE, IF APPLICABLE]
<!-- ☝️ Screenshot of your software (if applicable) via ![](https://uri-to-your-screenshot) ☝️ -->

[INSERT MORE DETAILED DESCRIPTION OF YOUR REPOSITORY HERE]
<!-- ☝️ Replace with a more detailed description of your repository, including why it was made and whom its intended for.  ☝️ -->

[INSERT LIST OF IMPORTANT PROJECT / REPO LINKS HERE]
<!-- example links>
[Website](INSERT WEBSITE LINK HERE) | [Docs/Wiki](INSERT DOCS/WIKI SITE LINK HERE) | [Discussion Board](INSERT DISCUSSION BOARD LINK HERE) | [Issue Tracker](INSERT ISSUE TRACKER LINK HERE)
-->

## Features

* [INSERT LIST OF FEATURES IMPORTANT TO YOUR USERS HERE]
  
<!-- ☝️ Replace with a bullet-point list of your features ☝️ -->

## Contents

* [Quick Start](#quick-start)
* [Changelog](#changelog)
* [FAQ](#frequently-asked-questions-faq)
* [Contributing Guide](#contributing)
* [License](#license)
* [Support](#support)

## Quick Start

This guide provides a quick way to get started with our project. Please see our [docs]([INSERT LINK TO DOCS SITE / WIKI HERE]) for a more comprehensive overview.

### What is Helm?

Helm is an application manager for Kubernetes. Think, Brew, Apt, or other package managers for servers, but for Kubernetes resources.
Kubernetes applications can become complicated in a hurry. 

- Pods
- Configmaps
- Secrets
- Environment variables
- L oad balancers
- Services 
and so on. Quite often you'll need some or all of the above. Helm can help you manage these resources, upgrade and update in lockstep with one another and extend your application capabilities with clever templates and run time configuration options that can set variables and similar without them being hardcoded into your pod or config definitions.

The other important thing we can do with Helm charts and the Unity platform is combine services from different parts of the Cloud infrastructure. For example, it might be easier for a project to allow AWS to manage Elasticsearch via their service, so rather than deploy an Elasticsearch pod, you might want to deploy Elasticsearch via the Unity specification and then link that Elasticsearch to the Kubernetes Pods in your Helm chart. This level of abstraction adds additional power to the Unity deployments, and interactions between Kubernetes and non Kubernetes services seamlessly.

### Requirements

* [INSERT LIST OF REQUIREMENTS HERE]
  
<!-- ☝️ Replace with a numbered list of your requirements, including hardware if applicable ☝️ -->

### Setup Instructions

#### How do I install Helm?

As there a number of ways to install Helm to develop against, we'll just link you to the docs rather than trying to rewrite them for this page. 

To install Helm check [this page](https://helm.sh/docs/intro/install/) from the Helm Documentation

### Run Instructions

1. [INSERT STEP-BY-STEP RUN INSTRUCTIONS HERE, WITH OPTIONAL SCREENSHOTS]

<!-- ☝️ Replace with a numbered list of your run instructions, including expected results ☝️ -->

### Usage Examples

#### How do I write a Helm chart?

A Helm chart is really just a collection of text files which explains to Helm how to install a selection of Kubernetes resources. In the simplest form they will have a Chart.yaml and a templates folder with various files in them. Templates are written to the chart install directory at run time and at that point are materialized, so any parameters passed in can be written to the template at that time. For example, you want a chart that can deploy a different version of a specific container, so you may want to pass the container tag in as a variable at which point its then added to the template to become a valid Kubernetes pod spec.

Of course, also, if your deployment is really simple, you don't need any templated variables at all, but Helm will also clean down used resources nicely, tell you whats installed on a cluster, where and which version, which can make managing these systems much cleaner.

The easiest way to get started is to use a template: `helm create my-unity-chart` and modify its contents from there!

#### How do I add my Helm chart to the repository?

To deploy your Chart to Unity, you need to have supplied it to our repository. This will make it available to our deployment service and to other consumers. The easiest way to do that is to 

- Fork this repository
- Create a branch in your fork and add your chart and all the associated files to the charts directory, ensure your chart has a unique name.
- Create a Pull Request
- Notify the Unity CS team that your PR is awaiting review.

Once the pull request is merged, your chart will then be available for installation on the Unity platform.

### Build Instructions (if applicable)

1. [INSERT STEP-BY-STEP BUILD INSTRUCTIONS HERE, WITH OPTIONAL SCREENSHOTS]

<!-- ☝️ Replace with a numbered list of your build instructions, including expected results / outputs with optional screenshots ☝️ -->

### Test Instructions (if applicable)

1. [INSERT STEP-BY-STEP TEST INSTRUCTIONS HERE, WITH OPTIONAL SCREENSHOTS]

<!-- ☝️ Replace with a numbered list of your test instructions, including expected results / outputs with optional screenshots ☝️ -->

## Changelog

See our [CHANGELOG.md](CHANGELOG.md) for a history of our changes.

See our [releases page]([INSERT LINK TO YOUR RELEASES PAGE]) for our key versioned releases.

<!-- ☝️ Replace with links to your changelog and releases page ☝️ -->

## Frequently Asked Questions (FAQ)

[INSERT LINK TO FAQ PAGE OR PROVIDE FAQ INLINE HERE]
<!-- example link to FAQ PAGE>
Questions about our project? Please see our: [FAQ]([INSERT LINK TO FAQ / DISCUSSION BOARD])
-->

<!-- example FAQ inline format>
1. Question 1
   - Answer to question 1
2. Question 2
   - Answer to question 2
-->

<!-- example FAQ inline with no questions yet>
No questions yet. Propose a question to be added here by reaching out to our contributors! See support section below.
-->

<!-- ☝️ Replace with a list of frequently asked questions from your project, or post a link to your FAQ on a discussion board ☝️ -->

## Contributing

Interested in contributing to our project? Please see our: [CONTRIBUTING.md](CONTRIBUTING.md)

## License

See our: [LICENSE](LICENSE)

## Support

[INSERT CONTACT INFORMATION OR PROFILE LINKS TO MAINTAINERS AMONG COMMITTER LIST]

<!-- example list of contacts>
Key points of contact are: [@github-user-1](link to github profile) [@github-user-2](link to github profile)
-->

<!-- ☝️ Replace with the key individuals who should be contacted for questions ☝️ -->

