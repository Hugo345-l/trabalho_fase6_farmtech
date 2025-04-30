# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
  <a href="https://www.fiap.com.br/"><img src="../assets/logo-fiap%20(1).png" alt="FIAP - Faculdade de Informática e Administração Paulista" border="0" width="40%" height="40%"></a>
</p>

<br>

# Projeto Visão Computacional

## 👨‍🎓 Integrantes
- [Bruno Castro - RM558359](https://www.linkedin.com/in/bruno-castro-dias/)
- [Hugo Mariano - RM560688](https://www.linkedin.com/in/hugomariano191628150/)
- [Matheus Castro - RM559293](https://www.linkedin.com/in/matheus-castro-63644b224/)

## 📜 Descrição

Este projeto aplica técnicas de visão computacional para detecção automática de objetos em imagens, com foco em modelos baseados em YOLO e CNN. O objetivo é comparar abordagens, avaliar desempenho e promover reprodutibilidade, com estrutura modular e documentação clara.

> 📓 **Notebook principal do projeto:**  
> [projeto_visao_computacional/notebooks/HugoMariano_rm560688_pbl_fase6.ipynb](projeto_visao_computacional/notebooks/HugoMariano_rm560688_pbl_fase6.ipynb)

---

## 📁 Estrutura do Repositório

A navegação do repositório está organizada para facilitar a localização de dados, modelos, resultados e experimentos. Veja abaixo o propósito de cada pasta principal:

- **projeto_visao_computacional/dataset/**  
  Estrutura de dados para detecção de objetos, organizada por classes e splits:
  - `train/`, `val/`, `test/`: Subpastas com imagens e labels para treino, validação e teste.
  - Cada classe possui sua própria subpasta, facilitando a expansão para novos objetos.
  - Os arquivos de labels seguem o padrão YOLO.

- **projeto_visao_computacional/models/**  
  Modelos treinados e arquivos relacionados:
  - `model_30epochs.pt`, `model_60epochs.pt`: Pesos dos modelos YOLO customizados.
  - `cnn_scratch/`: Modelos de CNN treinados do zero (`best_model.h5`, `final_model.h5`).
  - Subpastas como `yolo_30ep/`, `yolo_60ep/` armazenam checkpoints, métricas, gráficos e pesos intermediários.

- **projeto_visao_computacional/results/**  
  Resultados de experimentos e análises:
  - Gráficos de desempenho, matrizes de confusão, comparações entre modelos, CSVs de métricas e outputs de inferência.
  - Subpastas organizam resultados por abordagem (`cnn_scratch/`, `yolo_comparison/`, `comparison/`, etc).

- **projeto_visao_computacional/notebooks/**  
  Jupyter Notebooks com experimentos, análises e o notebook final do projeto:
  - `HugoMariano_rm560688_pbl_fase6.ipynb`: Notebook principal, documentando todo o fluxo do projeto, desde preparação dos dados até análise comparativa dos modelos.
  - Notebooks auxiliares para visualização e testes.

- **projeto_visao_computacional/config/**  
  Arquivos de configuração do projeto (ex: `data.yaml`), definindo classes, caminhos e parâmetros para treinamento.

- **projeto_visao_computacional/assets/**  
  Imagens e recursos visuais do projeto.

---

## 🚦 Orientações de Uso e Navegação

- **Reprodução de Experimentos**:  
  1. Instale as dependências:
     ```
     pip install -r requirements.txt
     ```
  2. Navegue até a pasta `projeto_visao_computacional/notebooks/` e execute o notebook principal para reproduzir todo o fluxo do projeto.
  3. Os dados necessários já estão organizados em `dataset/`.  
  4. Modelos treinados e resultados podem ser encontrados nas pastas `models/` e `results/`.

- **Resultados e Métricas**:  
  - Gráficos, CSVs e outputs de inferência estão em `results/`, organizados por abordagem e experimento.
  - Modelos finais e intermediários estão em `models/`.

- **Configuração**:  
  - Parâmetros de dataset e classes estão em `config/data.yaml`.

---

## 📚 Documentação e Referências

- O notebook principal (`notebooks/HugoMariano_rm560688_pbl_fase6.ipynb`) documenta todas as etapas, decisões e análises do projeto.
- Para detalhes sobre arquitetura, métricas e comparações, consulte as seções finais do notebook e os arquivos em `results/`.

---

## 🗃 Histórico de versões

- 1.1 - 30/04/2025 - Atualização final de estrutura e documentação.
- 1.0 - 30/04/2025 - Versão inicial.

## 📋 Licença

Este projeto segue o modelo educacional FIAP e está licenciado sob Creative Commons Attribution 4.0 International.
