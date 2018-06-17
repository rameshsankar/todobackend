FROM rameshsankar/todobackend-base:latest
MAINTAINER Ramesh Sankar <ramesh.sankar@gmail.com>

# Copy application
COPY target /wheelhouse

#Install application
RUN . /appenv/bin/activate && \
	pip install --no-index -f /wheelhouse todobackend && \
	rm -rf /wheelhouse
