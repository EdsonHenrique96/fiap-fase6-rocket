# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# Nome do projeto

## Nome do grupo

## 👨‍🎓 Integrantes: 
- <a href="https://www.linkedin.com/in/jonas-silva-0a659892/">Jonas Luis da Silva</a>
- <a href="https://www.linkedin.com/in/renan-francisco-de-paula-b3320915b/overlay/about-this-profile/">Renan Francisco de Paula</a>
- <a href="https://www.linkedin.com/in/jo%C3%A3o-vitor-severo-oliveira-87904134b/">João Vitor Severo Oliveira</a>
- <a href="https://www.linkedin.com/in/isagomesferreira/">Isabelle Gomes Ferreira</a>
- <a href="https://www.linkedin.com/in/edson-henrique-felix-batista-a00191123/">Edson Henrique Felix Batista</a>

## 👩‍🏫 Professores:
### Tutor(a) 
**Tutor:** <a href="https://www.linkedin.com/company/inova-fusca">Lucas Gomes Moreira</a>  
**Coordenador:** <a href="https://www.linkedin.com/company/inova-fusca">André Godoi Chiovato</a>


## 📜 Descrição

Projeto de visão computacional utilizando diferentes arquiteturas de CNN para classificar e identificar objetos em imagens.


## 📁 Estrutura do dataset

```
.
└── dataset
    ├── results
    ├── test
    │   ├── images
    │   └── labels
    ├── train
    │   ├── images
    │   └── labels
    └── valid
        ├── images
        └── labels
```

## 🔧 Como executar o código

1 - Crie o venv
2 - Execute o notebook do YOLO em ./yolo_model.ipynb
3 - Execute o notebook do Keras+Tensor Flow em ./cats_dogs_cnn.ipynp
4 - Execute o notebook do Darknet YOLO v3 em ./darknet_yolo.ipynp

## Considerações

Cada modelo foi avaliado considerando os seguintes aspectos:

### YOLOv5 
- **Facilidade de uso/integração:**
  - Fácil integração via pip install
  - API intuitiva e bem documentada
  - Suporte nativo para PyTorch
- **Precisão do modelo:**
  - mAP@0.5 de 0.74 (60 épocas)
  - Ótima detecção mesmo em imagens complexas
- **Tempo de treinamento:**
  - ~15 minutos para 30 épocas
  - ~30 minutos para 60 épocas
  - Treino eficiente em GPU
- **Tempo de inferência:**
  - ~0.02 segundos por imagem
  - Excelente para aplicações em tempo real

### CNN com Keras/TensorFlow
- **Facilidade de uso/integração:**
  - Interface de alto nível do Keras
  - Fácil implementação e customização
  - Boa integração com ecossistema TensorFlow
- **Precisão do modelo:**
  - Acurácia de teste ~85%
  - Bom para classificação binária simples
- **Tempo de treinamento:**
  - ~5 minutos para 20 épocas
  - Treino rápido para datasets pequenos
- **Tempo de inferência:**
  - ~0.01 segundos por imagem
  - Ótimo para classificação em lote

### Comparativo Final
- **YOLO** é mais adequado para:
  - Detecção de objetos em tempo real
  - Casos que exigem alta precisão
  - Projetos que necessitam localização do objeto
  
- **CNN Keras** é mais adequada para:
  - Classificação simples de imagens
  - Prototipagem rápida
  - Projetos com restrição de recursos computacionais

Ambos os modelos demonstraram bom desempenho para o dataset proposto, mas com diferentes características e casos de uso ideais.

## 📋 Licença

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>

