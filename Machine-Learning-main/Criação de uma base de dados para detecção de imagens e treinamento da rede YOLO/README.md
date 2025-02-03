# YOLOv5 - Criação de Uma Base de Dados e Treinamento da Rede YOLO

Este projeto utiliza o **YOLOv5** para realizar **Transfer Learning**, treinando um modelo personalizado baseado no **COCO Dataset**. O objetivo é adicionar novas classes ao modelo (Carro e pessoas) e aprimorar sua capacidade de detecção.

---

## 📌 Visão Geral
- **Objetivo**: Treinar um modelo YOLOv5 para identificar pessoas e carros em imagens.
- **Dataset**: Subconjunto do COCO 2017 (apenas classes "person" e "car").
- **Aplicações**: Sistemas de vigilância, análise de tráfego e projetos de IoT.

---

## 📌 Requisitos

Antes de começar, certifique-se de ter os seguintes requisitos instalados:

- **Python 3.8 ou superior**
- **PyTorch** (compatível com sua GPU/CPU)
- **Google Colab** (opcional, mas recomendado para uso com GPU)
- **YOLOv5** (da Ultralytics)
- **Google Drive** (para armazenar os modelos e dataset)

---

## 🛠️ Funcionalidades
- Pré-processamento de dados do COCO para formato YOLO
- Filtragem de classes específicas (pessoas e carros)
- Divisão automática do dataset (85% treino / 15% validação)
- Treinamento com transfer learning usando `yolov5s.pt`
- Detecção em tempo real via script

---

## 🧩 Tecnologias
- **YOLOv5** (Ultralytics)
- **Python 3.8+**
- **Google Colab**
- **Bibliotecas**:
  - OpenCV
  - PyTorch
  - Pandas/Numpy
  - Matplotlib