APP = helloworld
NAMESPACE = helloworld
PROD_VALUES = $(APP)/values-prod.yaml
QUALIF_VALUES = $(APP)/values-qualif.yaml


template:
	helm template $(APP) $(APP)/

template-prod:
	helm template $(APP) --values $(PROD_VALUES) $(APP)/

template-qualif:
	helm template $(APP) --values $(QUALIF_VALUES) $(APP)/

install:
	helm install $(APP) --namespace $(NAMESPACE) $(APP)/

install-prod:
	helm install $(APP) --namespace $(NAMESPACE) --values $(PROD_VALUES) $(APP)/

install-qualif:
	helm install $(APP) --namespace $(NAMESPACE) --values $(QUALIF_VALUES) $(APP)/

uninstall:
	helm uninstall $(APP)
