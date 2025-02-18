# Jupyter Notebook Project Template for Research software

This is a copier Jupyter Notebook project template that implements the best practices on sustainable software for researchers in Natural and Engineering Science. The template provides boilerplate folder structure, a Jupyter notebook, documentation, etc.

## How to Use

**Requirements**

- Python 3.11 or higher
- Copier

### Creating a software project

```shell
copier copy https://github.com/SS-NES/notebook-template <path/to/project-directory>
```
Alternatively, after clonning the repository, use a **full path** to `Software-Templates/`:

```shell
copier copy ~/<local-path>/Software-Templates <path/to/project-directory>
```

### Updating an existing project

Update the generated project by changing your answers. At the root of the software project, do:

```shell
copier update
```
> IMPORTANT: Before you are allow to update a project, the sofware project must be initialized as a Git repository, all files must be commited, and the status of the repository must show it is clean, i.e., no pending changes to commit.

### Creating a software project from an SMP

Given data from an SMP is provided as a YAML like:

```yml
project_name:  Demo
release_date: June 4, 2024
smp_version:  0.1.0
authors:  [Jane Doe](mailto:doe.j@example.nl)
purpose:  An example
research_project_context: software templates
ownership:  Institution
version_control:  git
public: True
reuse: False
repository: https://github.com
software_license: Apache-2.0 (Apache License 2.0)
citation: citation.cff
user_documentation: user.md
deployment_documentation: deploy.yml
testing:  testing.yml
quality:  Quality
packaging:  PyPI
maintenance:  maintenance.md
sustainability: sustainable.md
support:  support.md
risk_analysis:  No risk
data_management_plan: DMP
```

A  `smp.yml` file can be passed to copier when rendering the template.

```shell
copier copy --data-file </path/to/smp.yml> ~/<local-path>/Software-Templates <path/to/project-directory>
```

## Acknowledgements

- This template was inspired by [Cookiecutter Data Science](https://cookiecutter-data-science.drivendata.org)
