
FROM arm64v8/debian

RUN apt-get update && apt-get install -q -y --no-install-recommends \
    motion \
    jq

# Copy data
COPY run.sh /
COPY motion.conf /etc/

RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
