### Connect with SSH
    ssh <username>@192.168.55.1
    
### Add a data directory for the course with the following command in the Jetson Nano terminal you've logged into:  

    mkdir -p ~/nvdli-data
    
### To create and run a reusable script for this step try the following (example tag shown):

### create a reusable script
    echo "sudo docker run --runtime nvidia -it --rm --network host \
        --volume ~/nvdli-data:/nvdli-nano/data \
        --device /dev/video0 \
        nvcr.io/nvidia/dli/dli-nano-ai:v2.0.2-r32.7.1" > docker_dli_run.sh

### make the script executable
    chmod +x docker_dli_run.sh

### run the script
    ./docker_dli_run.sh
    
