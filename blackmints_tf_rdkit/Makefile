image_name=auroraywood/blackmints
tag_name=tf_rdkit

all:
	docker build --tag ${image_name}:${tag_name} .
	docker tag ${image_name}:${tag_name} ${image_name}:latest
	docker push ${image_name}:latest
	docker push ${image_name}:${tag_name}