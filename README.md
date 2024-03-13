# dagger-buildkite-plugin

BuildKite plugin to call a Dagger module. `dagger` is expected to be in the `PATH`.

## Example

Add the following to your `pipeline.yml`:

```yml
steps:
- plugins:
  - bcjio/dagger#main:
      module: github.com/shykes/daggerverse/hello@v0.1.2
      call: hello --name=buildkite
```

## Configuration

### `module` (Required, string)

The module to call.

### `call` (Required, string)

The call to make.

