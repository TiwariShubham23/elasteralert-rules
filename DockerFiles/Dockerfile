# GETTING BASE IMAGE
FROM ubuntu

RUN apt-get update
RUN apt-get install -y pip
RUN pip --version
RUN python3 --version
RUN apt-get install -y git
RUN git --version
RUN pip install elastalert
ADD "https://github.com/TiwariShubham23/elasteralert-rules.git" latest_commit
RUN git clone https://github.com/TiwariShubham23/elasteralert-rules.git
RUN ls elasteralert-rules
ARG host
# CMD python3 -m elastalert.elastalert --verbose --config elasteralert-rules/config.yml --rule elasteralert-rules/rules/example_frequency.yaml
CMD python3 --version