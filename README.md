# What is this?

Bitnami Matomo Docker image with GeoIP PECL preinstalled. Includes Dockerfile for building the custom Docker image, and the docker-compose file for spinning up a self-contained docker swarm.

## More Info

Assumes that the Matomo directory is mounted at /bitnami/matomo since this instance uses the bitnami/matomo docker image as a base.

The GeoIP PECL is preinstalled and initialized in php.ini. Still requires the GeoIPCity.dat or whatever database is being used to actually be downloaded into the Matomo install directory.

Docker image exists on Docker Hub [here](https://hub.docker.com/r/jameswang10/matomo_geoip/).

# Troubleshooting, Contributing

For any troubleshooting or contributions, please reference the base bitnami repo [here](https://github.com/bitnami/bitnami-docker-matomo).

If anything, this repo is just a basic reference on how to add PECL to the base image.

# License

All copyright and trademarks related to Bitnami and Matomo belongs to their respective holders.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

```
http://www.apache.org/licenses/LICENSE-2.0
```

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
