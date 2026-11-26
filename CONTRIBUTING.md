# Contributing to stratus

Thank you for helping. stratus aims to behave like AWS as the AWS SDKs see it, start in milliseconds and stay one
small binary; changes are weighed against those goals.

## Before you start

- **A bug** — open an issue with what you sent (SDK and version, or the request), what stratus answered and what AWS
  answers. A failing test is the best report.
- **A missing operation or service** — open an issue first, so that we can agree on its scope before you write it.
- **A security problem** — never in a public issue: see [SECURITY.md](SECURITY.md).

## Making a change

```sh
make test   # go test -race ./...
make lint   # gofmt and go vet
```

- Every service is tested through the real AWS SDK for Go: add a test that the SDK accepts the new behaviour,
  including its typed errors.
- Keep changes small and focused, one concern per pull request, with a description of what changes and why.
- Write commit messages as `type(scope): summary` (`feat`, `fix`, `perf`, `docs`, `test`, `chore`).
- Do not add a dependency without discussing it in the issue: stratus depends on the AWS SDK and a YAML parser only.

By contributing you agree that your contribution is licensed under the
[Apache License 2.0](https://github.com/stratus-emulator/stratus/blob/main/LICENSE), and you follow our
[Code of Conduct](CODE_OF_CONDUCT.md).
