FROM jupyter/base-notebook

USER root

# Install Java (OpenJDK), wget, unzip
RUN apt-get update && apt-get install -y openjdk-11-jdk wget unzip

# Download and install IJava kernel with proper registration
RUN wget 
https://github.com/SpencerPark/IJava/releases/download/v1.3.0/ijava-1.3.0.zip 
&& \
    unzip ijava-1.3.0.zip -d /tmp/ijava && \
    /tmp/ijava/install.sh --sys-prefix && \
    rm -rf /tmp/ijava ijava-1.3.0.zip

USER $NB_USER

