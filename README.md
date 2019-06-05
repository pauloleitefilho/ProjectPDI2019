# ProjectPDI2019
Projeto da disciplina de Processamento de imagens do Centro de Informática (Cin) da Universidade Federal de Pernambuco (UFPE)

########################
Alunos:
Geraldo Pires Junior
Paulo Fernando Leite Filho
########################

Alterações realizadas nos algoritmos do projeto 

Para rodar o Yolov3-keras-artigo
1- instalar os pacotes pythom:
python -m pip install opencv-python
python -m pip install Cython
python -m pip install Tensorflow
python -m pip install Keras
python -m pip install pydot
python -m pip install GraphViz
python -m pip install pycuda

via console: python -m pip install <pacote>

2 - Baixar os pesos (https://pjreddie.com/media/files/yolov3.weights) e colar na raiz Yolo3

2.1 - Rodar o comando: python yad2k.py cfg\yolo.cfg yolo3.weights data\yolo.h5 para atualizaçã odos pesos

3 - Executar o comando: python demo.py, para detecção dos objetos no filme, esta opção é uma demonstração do codigo de Yolo3.

4 - Para gerar as imagens de saida com as caixas delimitadoras: python demo.py --model cfg/yolo3.cfg --load yolo3/yolo.weights --imgdir sample_img --gpu 0.9 --json

5- A saida das imagens estão em imagens/res

 
#Como rodar o Yolo 2 
#Fonte: https://appliedmachinelearning.blog/2018/05/27/running-yolo-v2-for-real-time-object-detection-on-videos-images-via-darkflow/

# Clone the darkflow github repository:

git clone https://github.com/thtrieu/darkflow

#######################################
# Para rodar no Visual Studio Code no Windows10 
# Instala o Darkflow
python -m pip install -e .

#Instala os pacotes necessraios via terminal:
python -m pip install tensorflow 
python -m pip install opencv-python
python -m pip install cython
python -m pip install numpy

#Cython extensions in place.
python3 setup.py build_ext --inplace

# baixar os pesos YOLOv2 608x608 em:http://pjreddie.com/darknet/yolo/

# No arquivo de labels.txt completar as classes: https://github.com/nightrome/cocostuff/blob/master/labels.txt

#Criar o arquivo yolov2.cfg: https://github.com/pjreddie/darknet/blob/master/cfg/yolov2.cfg

#Rodar o comando: python flow --model cfg/yolov2.cfg --load bin/yolov2.weights --imgdir sample_img --gpu 0.9 --json

# Copiar as classes de coco,names para /cfg/yolov2.cfg

# A saida ser? aramzenada na pasta out
# As imagens para teste devem ser armazenadas em sample_img
 
