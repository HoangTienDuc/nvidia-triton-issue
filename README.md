# nvidia-triton-issue
python3: infer_trtis_backend.cpp:243: nvdsinferserver::SharedBatchBuf nvdsinferserver::TrtISBackend::allocateResponseBuf(const string&amp;, size_t, nvdsinferserver::InferMemType, int64_t): Assertion `buf->getTotalBytes() >= bytes' failed. Aborted (core dumped)


### Proceduce

1. With only triton_is:  nvcr.io/nvidia/tritonserver:21.02-py3
```
  Status: Success
  Logs: logs/triton.txt
```
2. With deepstream triton: nvcr.io/nvidia/deepstream:6.1-triton
```
  Status: False
  Logs: logs/deestream_triton.txtx
```
