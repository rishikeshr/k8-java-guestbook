# k8-java-guestbook

k8-java-guestbook is a sample Java guestbook application for demonstrating application autoinstrumentation with AppDynamics.
It uses __skaffold__ to build, run application on your target Kubernetes cluster. The default code was generated using Cloud Code plugin for Visual Studio Code.

## Installation

Clone this repository. Assuming that you have maven, java and skaffold configured in your environment, run the following commands.

The below command will build the image and push it to your Docker Hub repository. Please update the __skaffold.yml__ file to reflect your repository. Make sure you update the K8 manifest files to reflect your images. The files now reference the images in my repository.

To build your docker images, run the following command.
```bash
skaffold build
```

To deploy them in your target K8 cluster, use the below command. It will use your current cluster context.
```bash
skaffold run
```

For further options with skaffold, run the following command.
```bash
skaffold <command> --help
```


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[Apache](https://choosealicense.com/licenses/apache-2.0/)
