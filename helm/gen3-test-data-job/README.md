# gen3-test-data-job

![Version: 0.1.1](https://img.shields.io/badge/Version-0.1.1-informational?style=flat-square) ![Type: library](https://img.shields.io/badge/Type-library-informational?style=flat-square) ![AppVersion: 2022.10](https://img.shields.io/badge/AppVersion-2022.10-informational?style=flat-square)

A Helm chart for generating dummy data in gen3

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| fence.image | string | `"quay.io/cdis/fence:master"` |  |
| gentestdata.max_examples | string | `"10"` |  |
| gentestdata.submission_order | string | `"submitted_unaligned_reads"` |  |
| gentestdata.submission_user | string | `"cdis.autotest@gmail.com"` |  |
| gentestdata.test_program | string | `"DEV"` |  |
| gentestdata.test_project | string | `"test"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.0](https://github.com/norwoodj/helm-docs/releases/v1.11.0)
