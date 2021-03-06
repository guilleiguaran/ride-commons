RideCommons
===========

Curated set of common modules/functions used across multiple Ride projects in Elixir lang.

## Components

### RideCommons.HTTP

Based in HTTPoison. Responses are returned as tuples `{status_code, headers, body}` and errors are raised when bang versions (get!, post!, ...) of functions are used.

- get(url, headers)
- get!(url, headers)
- post(url, body, headers)
- post!(url, body, headers)
- put(url, body, headers)
- put!(url, body, headers)
- patch(url, body, headers)
- patch!(url, body, headers)
- delete(url, headers)
- delete!(url, headers)

Read [HTTPoison documentation](https://github.com/edgurgel/httpoison) for details.

### RideCommons.JSON

Based in exjsx. Labels decoded as atoms by default.

- encode(body, opts)
- encode!(body, opts)
- decode(body, opts)
- decode!(body, opts)

Read [exjsx documentation](https://github.com/talentdeficit/exjsx) for details about supported options.

### RideCommons.UUID

UUIDv4 generation using `:crypto.rand_bytes`

- generate_uuid

### RideCommons.Naming

Convenient functions for inflecting, copied from Mix.

- camelize(str)
- underscore(str)
