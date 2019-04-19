FROM mongo-express:0.49

COPY entrypoint.sh /
RUN chmod +x /entrypoint.sh && \
  npm install -g wait-port

ENTRYPOINT [ "tini", "--", "/entrypoint.sh" ]
CMD [ "mongo-express" ]
