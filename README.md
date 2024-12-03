[![Build and Push Docker Image](https://github.com/bwbioinfo/<tool>-docker-cwl/actions/workflows/build-and-push.yml/badge.svg)](https://github.com/bwbioinfo/<tool>-docker-cwl/actions/workflows/build-and-push.yml)

# tidyggplot2-docker

This repository provides a container to run [R] packages [tidyverse] and [ggplot2] based on [r-base] image. The tool is packaged in a Docker container, allowing it to run on any system with Docker or Singularity installed.

## Prerequisites

To use this tool, you must have the following software installed on your system:

- [Docker](https://www.docker.com/) OR [Singularity](https://sylabs.io/singularity/) OR [Apptainer](https://apptainer.org/)

## Installation

To install and run the tool, follow these steps:

1. Clone this repository to your local machine.
2. Install Docker, if you haven't already done so.
3. (optional) Build the Docker image by running the following command from the root of the repository:

    ```
    docker build -f docker/Dockerfile -t tidyggplot2 .
    ```
    OR pull from the built container.
    ```
    docker pull ghcr.io/charlenelawdes/tidyggplot2-docker:latest
    ```

## Usage

To run the docker container, you will need to use:

```
docker run -it tidyggplot2-docker
```

To see how to mount directories within containers and other useful `docker run` options, see [Docker] documentation (https://docs.docker.com/reference/cli/docker/container/run).

## Contributing

If you wish to contribute to this project, please follow the standard GitHub workflow:

1. Fork the repository
2. Create a new branch for your changes
3. Make your changes and commit them
4. Push your changes to your fork
5. Submit a pull request to this repository

## License

This project is licensed under the [MIT License](https://github.com/bwbioinfo/tool-docker-cwl/blob/main/LICENSE).

## Contact

If you have any questions or feedback, please contact the author via GitHub.

[Docker]: https://www.docker.com
[Singularity]: https://docs.sylabs.io/guides/3.5/user-guide/introduction.html
[Apptainer]: https://apptainer.org
[R]: https://www.r-project.org/
[tidyverse]: https://www.tidyverse.org/
[ggplot2]: https://ggplot2.tidyverse.org/
[r-base]: https://hub.docker.com/_/r-base
