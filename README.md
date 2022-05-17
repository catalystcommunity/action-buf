<!-- start title -->

# GitHub Action:Action Buf

<!-- end title -->
<!-- start description -->

Runs buf commmands to lint and generate protos

<!-- end description -->
<!-- start contents -->
<!-- end contents -->
<!-- start usage -->

```yaml
- uses: catalystsquad/action-buf@undefined
  with:
    # Buf user
    buf-user: ""

    # Buf token
    buf-token: ""

    # Git token to use
    # Default: ${{ github.token }}
    token: ""

    # Subdirectory to use with buf push
    # Default: .
    push-dir: ""

    # Ref to checkout
    # Default: ${{ github.head_ref }}
    ref: ""

    # Run `buf lint`
    # Default: true
    lint: ""

    # Run `buf generate`
    # Default: true
    generate: ""

    # Generate typescript types. If true, @grpc/proto-loader will be used to generate
    # grpc stubs and typescript types, and output to dist/nodejs
    # Default: true
    generate-typescript: ""

    # Space delineated string of paths from project root to proto files to generate
    # typescript types for.
    # Default:
    generate-typescript-protos: ""

    # Run `buf breaking`
    # Default: true
    breaking: ""

    # Run `buf mod prune`
    # Default: true
    mod-prune: ""

    # Run `buf mod update`
    # Default: true
    mod-update: ""

    # Run `buf push`
    # Default: false
    push: ""

    # Arguments to pass to proto loader (https://www.npmjs.com/package/@grpc/proto-loader)
    # Default: --keepCase --longs=String --enums=String --defaults --oneofs --grpcLib=@grpc/grpc-js
    ts-proto-args: ""
```

<!-- end usage -->
<!-- start inputs -->

| **Input**                        | **Description**                                                                                                                            |                                      **Default**                                       | **Required** |
| :------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------: | :----------: |
| **`buf-user`**                   | Buf user                                                                                                                                   |                                                                                        |   **true**   |
| **`buf-token`**                  | Buf token                                                                                                                                  |                                                                                        |   **true**   |
| **`token`**                      | Git token to use                                                                                                                           |                                 `${{ github.token }}`                                  |  **false**   |
| **`push-dir`**                   | Subdirectory to use with buf push                                                                                                          |                                          `.`                                           |  **false**   |
| **`ref`**                        | Ref to checkout                                                                                                                            |                                `${{ github.head_ref }}`                                |  **false**   |
| **`lint`**                       | Run `buf lint`                                                                                                                             |                                         `true`                                         |  **false**   |
| **`generate`**                   | Run `buf generate`                                                                                                                         |                                         `true`                                         |  **false**   |
| **`generate-typescript`**        | Generate typescript types. If true, @grpc/proto-loader will be used to generate grpc stubs and typescript types, and output to dist/nodejs |                                         `true`                                         |  **false**   |
| **`generate-typescript-protos`** | Space delineated string of paths from project root to proto files to generate typescript types for.                                        |                                                                                        |  **false**   |
| **`breaking`**                   | Run `buf breaking`                                                                                                                         |                                         `true`                                         |  **false**   |
| **`mod-prune`**                  | Run `buf mod prune`                                                                                                                        |                                         `true`                                         |  **false**   |
| **`mod-update`**                 | Run `buf mod update`                                                                                                                       |                                         `true`                                         |  **false**   |
| **`push`**                       | Run `buf push`                                                                                                                             |                                        `false`                                         |  **false**   |
| **`ts-proto-args`**              | Arguments to pass to proto loader (https://www.npmjs.com/package/@grpc/proto-loader)                                                       | `--keepCase --longs=String --enums=String --defaults --oneofs --grpcLib=@grpc/grpc-js` |  **false**   |

<!-- end inputs -->
<!-- start outputs -->

| **Output**      | **Description** | **Default** | **Required** |
| :-------------- | :-------------- | ----------- | ------------ |
| `random-number` | Random number   |             |              |

<!-- end outputs -->
<!-- start examples -->

### Example usage on release to push to BSR

```yaml
name: Push protos to buf
on:
  release:
    types: [created]
jobs:
  buf-push:
    name: Push protos to buf bsr
    runs-on: ubuntu-latest
    steps:
      - uses: crazy-max/ghaction-dump-context@v1
      - uses: catalystsquad/action-buf@v1
        with:
          token: ${{ secrets.AUTOMATION_PAT }}
          buf-user: ${{ secrets.BUF_USER }}
          buf-token: ${{ secrets.BUF_TOKEN }}
          lint: false
          generate: false
          breaking: false
          mod-prune: false
          mod-update: false
          push: true
```

<!-- end examples -->
<!-- start [.github/ghdocs/examples/] -->
<!-- end [.github/ghdocs/examples/] -->
