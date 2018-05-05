FROM java:8u111-jre-alpine

WORKDIR /app
ENV HAZELCAST_SERVICE=hazelcast\
    POD_NAMESPACE=default \
    DNS_DOMAIN=cluster.local \
    KUBERNETES_MASTER=https://kubernetes.default.svc.cluster.local

COPY *.jar .

EXPOSE 5701

CMD ["sh", "-c", "java -jar *.jar"]
