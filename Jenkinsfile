node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'DockerId') {

        def customImage = docker.build("ankimittal/add")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
