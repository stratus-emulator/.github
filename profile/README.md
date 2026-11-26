# stratus

**A fast local emulator of the AWS services your application needs in development and tests.**
One static Go binary, ready in milliseconds, with the resources you declare in a manifest.

- **SQS, S3, DynamoDB, Kinesis and Step Functions** on one port, `:4566`, for any AWS SDK or the AWS CLI.
- **Resources are declared, not scripted**: a YAML manifest lists what exists at start.
- **A web panel** to watch, search and change what the emulator holds, including Kinesis records aggregated by the Kinesis Producer Library.
- **Built for tests**: reset between suites, or run it inside a Go test with no container.

```sh
docker run --rm -p 4566:4566 stratusemulator/stratus
```

Start at [stratus-emulator/stratus](https://github.com/stratus-emulator/stratus). Questions and ideas go to
[Discussions](https://github.com/stratus-emulator/stratus/discussions); contributions are welcome, read
[how to contribute](https://github.com/stratus-emulator/.github/blob/main/CONTRIBUTING.md) first.
If stratus saves you time, you can [sponsor its maintainer](https://github.com/sponsors/ODudek).
