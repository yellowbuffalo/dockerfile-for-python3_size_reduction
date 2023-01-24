# Python3 Dockerfile with Two-stage Size Reduction
The dockerfile is to build a python3 environment with two-stage size reduction.
| Version  | Base Image | Method | Size |
| ------------- | ------------- | ------------- | ------------- |
| python39  | python:3.9  | -  | 1GB  |
| python39_slim  | python:3.9-slim  | -  | 210MB  |
| python39_slim_multi_stage  | Build:python:3.9-slim; Dependency: python3-distroless  | multi-stage  | 130MB  |
