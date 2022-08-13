node {

    checkout scm

    docker.withRegistry('https://github.com/itamargabay1607/dockerwebapp.git', 'dockerHub') {

        def customImage = docker.build("docker-pipeline")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
