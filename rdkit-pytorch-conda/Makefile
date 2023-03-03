image_name=auroraywood/aidd
tag_name=ubuntu20.04-rdkit-pytorch1.8.2-py37-cuda11-conda-base

all:
	docker build --tag ${image_name}:${tag_name} .
	docker tag ${image_name}:${tag_name} ${image_name}:latest
	docker push ${image_name}:latest
	docker push ${image_name}:${tag_name}