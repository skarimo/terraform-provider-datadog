# datadog-api-client-go

[![codecov](https://codecov.io/gh/DataDog/datadog-api-client-go/branch/master/graph/badge.svg?token=9Vx8eU0VlA)](https://codecov.io/gh/DataDog/datadog-api-client-go)

This repository contains a Go API client for the [Datadog API](https://docs.datadoghq.com/api/).
The code is generated using [openapi-generator](https://github.com/OpenAPITools/openapi-generator)
and [apigentools](https://github.com/DataDog/apigentools).

## Layout

This repository contains per-major-version API client packages. Right
now, Datadog only has one API version - `v1` - so that is the only module present. If/when
there is another version of the API, we will add a different package for it. The end goal is
to be able to use API clients for different major versions of the API side-by-side.

## The Datadog API v1 Client

The client library for Datadog API v1 is located in the `api/v1/datadog` directory. Import it with

```go
import "github.com/DataDog/datadog-api-client-go/api/v1/datadog"
```

All the documentation for this package is available through `api/v1/datadog/README.md`.

## Contributing

As most of the code in this repository is generated, we will only accept PRs for files
that are not modified by our code-generation machinery (changes to the generated files
would get overwritten). We happily accept contributions to files that are listed in:


as well as tests files:

