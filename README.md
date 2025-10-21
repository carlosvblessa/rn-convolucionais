# Redes Neurais Convolucionais — Formação Deep Learning com PyTorch

Este repositório reúne os notebooks trabalhados no curso **Redes Neurais Convolucionais** da formação *Deep Learning com PyTorch* (Alura). O material cobre desde a intuição da operação de convolução até diferentes estratégias de treino com redes convolucionais completas.

## Configuração do ambiente

1. Recomendado: criar e ativar um ambiente virtual (`python -m venv .venv && source .venv/bin/activate` no Linux/macOS ou `.venv\\Scripts\\activate` no Windows).
2. Instalar as dependências com `pip install -r requirements.txt`.
3. Abrir os notebooks com `jupyter notebook` ou `jupyter lab`.

> Os datasets utilizados (MNIST, Pascal VOC, CIFAR10, entre outros) são baixados automaticamente pelas chamadas do `torchvision` na primeira execução das células correspondentes. As funções do `skimage` utilizam imagens de demonstração da própria biblioteca.

## Conteúdo dos notebooks

- `01-Datasets.ipynb`: apresenta problemas de classificação, detecção e segmentação; demonstra como carregar MNIST e Pascal VOC com `torchvision.datasets` e discute implicações nas camadas de saída das redes.
- `02-Convolucao1D.ipynb`: explora a convolução 1D em sinais simulados (exemplo de acelerômetro), ilustrando o efeito de kernels ao longo do tempo.
- `03-Convolucao2D.ipynb`: migra o conceito para imagens, aplicando diferentes kernels 2D em exemplos do `skimage` para destacar padrões como bordas.
- `03-Filtros.ipynb`: revisita filtros convolucionais clássicos, mostrando exemplos práticos de kernels projetados manualmente e seus mapas de ativação.
- `04-Conv2d.ipynb`: estuda a camada `torch.nn.Conv2d`, configurando parâmetros chave (canais, kernel size, stride, padding) e analisando a transformação dos tensores.
- `05-OutrasCamadas.ipynb`: complementa o pipeline com camadas auxiliares (pooling, batch normalization) e examina seus efeitos em imagens de exemplo.
- `06-Estrategias.ipynb`: compara estratégias de treino com CNNs — do zero, extração de características e fine-tuning — usando modelos pré-treinados do `torchvision.models`.
- `06-TreinoDoZero.ipynb`: implementa uma CNN inspirada na LeNet-5 para o CIFAR10, cobrindo data loaders, treinamento supervisionado, métricas e avaliação.

## Sugestão de estudo

O conteúdo foi organizado para ser percorrido na ordem numérica dos notebooks. Assim, a base conceitual sobre convoluções alimenta a construção de redes cada vez mais completas até chegar às estratégias de treino avançadas.

