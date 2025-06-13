# image-processing

Pacote Python para processamento e manipulação de imagens usando scikit-image.

O pacote image_processing é usado para:

**Processing:**

- Histogram matching
- Structural similarity
- Resize image

**Utils:**

- Read image
- Save image
- Plot image
- Plot result

## Instalação

Use o gerenciador de pacotes [pip](https://pip.pypa.io/en/stable/) para instalar image-processing

```bash
pip install image-processing
```

## Dependências

Este pacote requer as seguintes bibliotecas:

- matplotlib
- numpy
- scikit-image >= 0.16.1

Para instalar as dependências:

```bash
pip install -r requirements.txt
```

## Uso

### Módulo Processing

```python
from image_processing.processing import combination, transformation

# Histogram matching
combination.find_histogram_match(image1, image2)

# Structural similarity
combination.calculate_structural_similarity(image1, image2)

# Resize image
transformation.resize_image(image, new_size)
```

### Módulo Utils

```python
from image_processing.utils import io, plot

# Read and save images
image = io.read_image("path/to/image.jpg")
io.save_image(image, "path/to/output.jpg")

# Plot images and results
plot.plot_image(image)
plot.plot_result(original, processed)
plot.plot_histogram(image)
```

## Estrutura do Projeto

```
image_processing/
├── processing/
│   ├── combination.py      # Histogram matching, Structural similarity
│   └── transformation.py   # Resize image
└── utils/
    ├── io.py              # Read/Save image functions
    └── plot.py            # Plot image, Plot result functions
```

## Contribuição

Pull requests são bem-vindos. Para mudanças importantes, abra uma issue primeiro para discutir o que você gostaria de alterar.

## Autor

AgathaCRuiz

## License

[MIT](https://choosealicense.com/licenses/mit/)
