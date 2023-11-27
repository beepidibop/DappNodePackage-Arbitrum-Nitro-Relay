ARG UPSTREAM_VERSION

FROM offchainlabs/nitro-node:${UPSTREAM_VERSION}

USER root

USER user

ENTRYPOINT relay --node.feed.output.addr=0.0.0.0 \
  --node.feed.input.url=$FEED_INPUT_URL \
  --node.feed.output.port=$FEED_OUTPUT_PORT \
  --chain.id=42161 \
  $EXTRA_OPTS