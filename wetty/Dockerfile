FROM ghcr.io/mastodon/mastodon

RUN yarn global add wetty

CMD ["bash","-c","wetty -p $PROT --ssh-pass $SSH_PASS"]
