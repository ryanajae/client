# The BugSwarm Client

![The BugSwarm Mascot](https://cloud.githubusercontent.com/assets/8139148/24324903/1101b9a2-114c-11e7-9340-316022ef57d5.png)

A command line client to interface with the [BugSwarm](https://bugswarm.github.io) artifact collection.

## Getting Started

### Installation
> Requires Python 3.

```
$ pip3 install bugswarm-client
```

### Uninstallation
```
$ pip3 uninstall bugswarm-client
```

### Usage
- Download a Docker image and enter the Docker container associated with an artifact. Choose an image tag from the [website](http://bugswarm.org/artifact-browser) or via the [REST API](https://github.com/BugSwarm/database#api-endpoints). The script argument is a path to an executable in the container's filesystem that will be executed inside the container.
    ```
    $ bugswarm run --image-tag <image_tag> [--script <script>]
    ```
- Show metadata for an artifact.
    ```
    $ bugswarm show --image-tag <image_tag>
    ```
- Show usage text.
    ```
    $ bugswarm --help
    ```

### Development
1. Clone this repository.
    ```
    $ git clone https://github.com/BugSwarm/client.git
    ```
1. `cd` into the root directory of this repository.
    ```
    $ cd client
    ```
1. Install the tool.
    ```
    $ sudo -H pip3 install --upgrade --force-reinstall --process-dependency-links -e .
    ```
Modifications to the source are automatically reflected when the tool is invoked.
