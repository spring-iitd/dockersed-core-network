# Dockerised-Core-Network

This repo is to simplify our core network deployment using docker containers. We are using the following submodules in the repository:

1. [Open5GS](https://github.com/Borjis131/docker-open5gs)
2. [Free5GC](https://github.com/free5gc/free5gc-compose)
3. [OpenAirInterface Core Network](https://gitlab.eurecom.fr/oai/cn5g/oai-cn5g-fed)
4. [UERANSIM](https://github.com/louisroyer-docker/ueransim)

The other dirctories are as follows:

- `./configurations/` has files specific to a deployment that has been tested and runs. There can be some path dependencies that you might need to change.
- `./shared/` is shared between the VMs and the host machine.
- `./docs/` has some documentation that might be useful.
- `./scripts/` has some scripts that might be useful.

> Please note while cloning the you need to use the '--recursive-submodule flag':

```bash
git clone --recursive-submodule https://github.com/spring-iitd/dockersed-core-network 
```

Please note, the changes you are making in the submodules would reflect in the host repository. I would recommend following keeping your changes in this repository only and not in the sub-dirctories.
