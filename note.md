```bash
sudo -E docker build -t synobuild .
sudo -E docker run --rm --privileged --network=host --env http_proxy=http://127.0.0.1:8889 --env https_proxy=http://127.0.0.1:8889 --env PACKAGE_ARCH=armada37xx --env DSM_VER=7.2 -v $(pwd)/artifacts:/result_spk synobuild
```
