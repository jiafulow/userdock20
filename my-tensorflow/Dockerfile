FROM tensorflow/tensorflow:latest

RUN apt-get update && apt-get install --no-install-recommends -y \
        curl \
        git \
        wget

RUN python3 -m pip --no-cache-dir install --upgrade \
        pip \
        setuptools

RUN python3 -m pip --no-cache-dir install \
        tensorflow==2.2.0 \
        tensorflow-probability==0.10.0 \
        neural-structured-learning==1.2.0

RUN python3 -m pip --no-cache-dir install \
        jupyter \
        matplotlib \
        seaborn

RUN python3 -m ipykernel.kernelspec

EXPOSE 8888

#ADD entrypoint.sh /entrypoint.sh
#RUN chmod 755 /entrypoint.sh

#ENTRYPOINT ["/entrypoint.sh"]
