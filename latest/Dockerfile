FROM mravenel/alpine

ENV HUGO_VERSION '0.25'
ENV HUGO_SHA '443b6d2af0df8469a3c853acac03ddfb66ce05c642342edf3813f5c55e3b2f95'

RUN wget -O $HUGO_VERSION.tar.gz https://github.com/spf13/hugo/releases/download/v$HUGO_VERSION/hugo_${HUGO_VERSION}_Linux-64bit.tar.gz \
    && echo "$HUGO_SHA  $HUGO_VERSION.tar.gz" | sha256sum -c \
    && tar xf $HUGO_VERSION.tar.gz && mv hugo* /usr/bin/hugo \
    && rm $HUGO_VERSION.tar.gz