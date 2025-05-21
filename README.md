  # Qlty Git Source

  This repository serves as a public Qlty git source that provides an example of a standardized static analysis
  configuration that can be shared across multiple repositories.

  ## Using this Git Source

  Add the following configuration to your `qlty.toml` file:

  ```toml
  [[source]]
  name = "qlty-source"
  repository = "https://github.com/qltysh/qlty-source"
  tag = "v0.0.1" # or use latest tag
  ```

  Alternatively, you can use a branch instead of a tag:

```toml
  [[source]]
  name = "example-source"
  repository = "https://github.com/username/repo-name"
  branch = "main"
```

Using one vs the other will depend on whether you want repositories to "opt-in" to changes in the standarized config (by bumping the tag), or receive them automatically (by specifying a branch). 
