### common

````yaml

  ---
  # name of this project
  name: readme

  # License of this project
  license: 'MIT'

  email:
    support: support@hadenlabs.com

  # Canonical GitHub repo
  github_repo: hadenlabs/readme

  # Badges to display
  badges:
    - name: 'Build Status'
      image: 'https://travis-ci.org/hadenlabs/readme.svg?branch=main'
      url: 'https://travis-ci.org/hadenlabs/readme'

  # Short description of this project
  description: |-
    examples of readme generator by gotemplate.

  # load examples
  examples:
    - 'docs/examples/common.md'

  # How to use this project
  usage: |-

    ```bash
      example of use
    ```

````

### GitHub Repo

```yaml
# Github Repo to this project
github_repo: hadenlabs/readme
```

### GitLab Repo

```yaml
# GitLab Repo to this project
gitlab_repo: hadenlabs/readme
```

### Custom GitLab Repo

```yaml
# GitLab Repo to this project
gitlab_host: gitlab.domain.com
gitlab_repo: hadenlabs/readme
```

### Copyrights

```yaml
# copyrights to this project
copyrights:
  - name: 'hadenlabs'
    url: 'https://hadenlabs.com'
    year: '2018'
```

### TO-DO

```yaml
todo:
  - name: 'chore: implement features'
    url: 'https://github.com/hadenlabs/readme/issues/4'
```

### Features

```yaml
features:
  - 'information of feature'
```

### screenshots

```yaml
screenshots:
  - name: 'name screentshot'
    url: 'url image'
    description: 'decription of screenshots'
```

### introduction

```yaml
introduction: |-

  example of introduction
```

### usage

```yaml
usage: |-

  example of usage
```

### Quick Start

```yaml
quickstart: |-

  example of quick start
```

### requirements

```yaml
requirements: |-

  This is a list of requirements that need to be installed previously to enjoy all the goodies of this configuration:

  * [gomplate](https://github.com/hairyhenderson/gomplate)
```

### Installation

```yaml
installation:
  - 'path of file'
```

### examples

```yaml
examples:
  - 'path of file'
```

### Related Projects

```yaml
related:
  - name: 'name project related'
    url: 'project related'
    description: 'description of project related'
```

### References

```yaml
references:
  - name: 'name project references'
    url: 'project references'
    description: 'description of project references'
```

### contributors

```yaml
# Contributors to this project
contributors:
  - name: 'Luis Mayta'
    github: 'luismayta'
```
