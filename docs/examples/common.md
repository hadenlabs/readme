### common

```hcl

  module "main" {
      source = "hadenlabs/repository/github"
      version = "0.7.2"

      providers = {
        github = github
      }

      name        = "repository-example"
      description = "github repository for repository"
      visibility  = "public"
      settings = {
        auto_init              = true
        has_issues             = true
        has_wiki               = true
        has_projects           = true
    }
  }

```

### implement key deploy

```hcl

  module "main_with_key" {
    source = "hadenlabs/repository/github"
    version = "0.7.2"

    providers = {
      github = github
    }

    name        = "repository-example-with-key"
    description = "github repository for repository"
    visibility  = "public"
    deploy_keys = [{
      title = "user key"
      key = "/usr/etc/key/user.pub"
      read_only = false
    }]
  }

```

### implement secrets

```hcl

  module "main_with_secrets" {
    source = "hadenlabs/repository/github"
    version = "0.7.2"

    providers = {
      github = github
    }

    name        = "repository-example-with-key"
    description = "github repository for repository"
    visibility  = "public"
    secrets = {
      key= value
    }
  }
```

### implement pages

```hcl

  module "main_with_pages" {
    source = "hadenlabs/repository/github"
    version = "0.7.2"

    providers = {
      github = github
    }

    name        = "repository-example-with-key"
    description = "github repository for repository"
    visibility  = "public"
    pages = {
      branch = "gh-pages"
      path = "/"
    }

    topics = [
        "go",
        "terraform",
    ]

    settings = {
      has_wiki               = true
      has_projects           = true
      vulnerability_alerts   = true
    }
  }

```

### implement templates

```hcl

  module "main" {
      source = "hadenlabs/repository/github"
      version = "0.7.2"

      providers = {
        github = github
      }

      name        = "repository-example"
      description = "github repository for repository"
      visibility  = "public"
      settings = {
        auto_init              = true
        has_issues             = true
        has_wiki               = true
        has_projects           = true
      }

      pages = {
        owner = "owner-user"
        repository = "name-repository"
      }
  }

```

### implement collaborator

```hcl

  module "main" {
      source = "hadenlabs/repository/github"
      version = "0.7.2"

      providers = {
        github = github
      }

      name        = "repository-example"
      description = "github repository for repository"
      visibility  = "public"
      settings = {
        auto_init              = true
        has_issues             = true
        has_wiki               = true
        has_projects           = true
      }

      collaborators = [
      {
        username = "other-user"
        permission = "push"
      },
      ]
  }

```