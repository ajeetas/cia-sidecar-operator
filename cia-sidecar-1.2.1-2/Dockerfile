# Build the manager binary
FROM quay.io/operator-framework/helm-operator:v1.0.1

LABEL name="Citrix-cpx-istio-sidecar-injector-operator" \
      vendor="Citrix" \
      version="v1.2.1" \
      release="1" \
      summary="This is Citrix cpx istio sidecar injector operator helm operator." \
      description="This operator will deploy Citrix cpx istio sidecar injector to the cluster."

COPY licenses /licenses


ENV HOME=/opt/helm
COPY watches.yaml ${HOME}/watches.yaml
COPY helm-charts  ${HOME}/helm-charts
WORKDIR ${HOME}
