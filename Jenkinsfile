node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("horse00/docker_webapp_demo")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
