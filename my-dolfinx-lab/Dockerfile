FROM dolfinx/lab:v0.10.0

USER root

COPY requirements.txt /tmp/requirements.txt

RUN apt-get update && apt-get install -y calculix-ccx
RUN python3 -m pip install -r /tmp/requirements.txt
