# For any container to run it must have minimal OS, it doesn't need to be a full OS
# So, for that purpose we will first select an OS image that is suitable for our tasks
FROM ubuntu:latest

# Once we select the image, all the steps of our workflow now going to be happening in that image
# So, we will create a working directory in that image
WORKDIR /work_dir_in_img

#Then we will copy all the required files from our host OS to the image that we are using for our tasks execution 
COPY . /work_dir_in_img

# install all the required packages that will be needed for the tasks execution
RUN apt-get update
RUN apt-get install -y python3
RUN apt-get install -y python3-pip


CMD ["python3", "app.py"]
