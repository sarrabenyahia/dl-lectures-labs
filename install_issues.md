# 1. Si le terminal se ferme au moment d'activate

conda uninstall -n dl-lectures-env keras tensorflow
activate dl-lectures-env
pip install "keras==2.1.*" "tensorflow==1.4.*"


# 2. Sinon (dans l'environnement pas défault)

conda install "keras==2.1.*" "tensorflow==1.4.*"
