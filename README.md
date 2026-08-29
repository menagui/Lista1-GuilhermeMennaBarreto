# Lista 1 - Guilherme Menna Barreto

Este repositório contém exemplos e códigos utilizados na disciplina de **Processamento Gráfico: Fundamentos** do curso Ciência da Computação da Unisinos. Ele é estruturado para facilitar a organização dos arquivos e a compilação dos projetos utilizando CMake.

## 📂 Estrutura do Repositório

```plaintext
📂 PG2026-2/
├── 📂 include/                # Cabeçalhos e bibliotecas de terceiros
│   ├── 📂 glad/               # Cabeçalhos da GLAD (OpenGL Loader)
│   │   ├── glad.h
│   │   ├── 📂 KHR/            # Diretório com cabeçalhos da Khronos (GLAD)
│   │       ├── khrplatform.h
├── 📂 common/                 # Código reutilizável entre os projetos
│   ├── glad.c                 # Implementação da GLAD
├── 📂 src/                    # Código-fonte dos exemplos e exercícios
│   ├── 📁 Exemplos/           # Pasta reservada para exemplos dados em aula
│   └── 📂 Exercicios/
│       └── 📂 Lista1/
│           ├── 📄 README.md   # Índice dos itens implementados
│           ├── 📂 Exercicio1/ # Itens 1a até 1d
│           ├── 📂 Exercicio2/ # Itens 2a até 2d
│           ├── 📂 Exercicio3/ # Respostas descritivas no README
│           └── 📂 Exercicio4/ # Desenho de uma casa com primitivas
├── 📂 build/                 # Diretório gerado pelo CMake (não incluído no repositório)
├── 📄 CMakeLists.txt         # Configuração do CMake para compilar os projetos
├── 📄 README.md              # Este arquivo, com a documentação do repositório
├── 📄 GettingStarted.md      # Tutorial detalhado sobre como compilar usando o CMake
├── 📄 ...
```

Siga as instruções detalhadas em [GettingStarted.md](GettingStarted.md) para configurar e compilar o projeto.

## Lista de exercícios

A organização e a descrição dos itens implementados na Lista 1 estão disponíveis em [`src/Exercicios/Lista1/README.md`](src/Exercicios/Lista1/README.md).

## ⚠️ **IMPORTANTE: Baixar a GLAD Manualmente**
Para que o projeto funcione corretamente, pode ser necessário **baixar a GLAD manualmente** utilizando o **GLAD Generator**.

### 🔗 **Acesse o web service do GLAD**:
👉 [GLAD Generator](https://glad.dav1d.de/)

### ⚙️ **Configuração necessária:**
- **API:** OpenGL  
- **Version:** 3.3+ (ou superior compatível com sua máquina)  
- **Profile:** Core  
- **Language:** C/C++  

### 📥 **Baixe e extraia os arquivos:**
Após a geração, extraia os arquivos baixados e coloque-os nos diretórios correspondentes:
- Copie **`glad.h`** para `include/glad/`
- Copie **`khrplatform.h`** para `include/glad/KHR/`
- Copie **`glad.c`** para `common/`

🚨 **Sem esses arquivos, a compilação falhará!** É necessário colocar esses arquivos nos diretórios corretos, conforme a orientação acima.

---

## 📚 Sugestão de Estrutura para seu próprio repositório

Recomendamos que você crie um repositório próprio, estruturado com subdiretórios dentro de `src`, para organizar suas atividades da disciplina:

```
📁 PG2026-2/
├── 📁 src/
│   ├── 📁 Exemplos/
│   │   └── ...
│   └── 📁 Exercicios/
│       ├── 📁 Lista1/
│       │   ├── 📁 Ex1/
│       │   │   └── main.cpp
│       │   ├── 📁 Ex2/
│       │   │   └── main.cpp
│       │   ├── 📁 Ex3/
│       │   │   └── main.cpp
│       │   └── README.md
│       ├── 📁 Lista2/
│       │   ├── 📁 Ex1/
│       │   │   └── main.cpp
│       │   ├── 📁 Ex2/
│       │   │   └── main.cpp
│       │   ├── 📁 Ex3/
│       │   │   └── main.cpp
│       │   └── README.md
│       ├── 📁 TrabalhoGrauA/
│       │   ├── main.cpp
│       │   ├── Object.cpp
│       │   ├── Object.h
│       │   ├── Shader.cpp
│       │   ├── Shader.h
│       │   └── README.md
│       └── ...
├── 📁 include/ # Cabeçalhos comuns (se necessário)
├── 📁 common/  # Arquivos comuns (como glad.c)
├── 📄 CMakeLists.txt
└── 📄 README.md
```
> Você pode alterar a estrutura dos diretórios, mas sempre que o fizer, adicione-os corretamente no CMakelists.txt.
> Cada diretório dentro de `src/` pode conter um arquivo `README.md` com informações específicas sobre a atividade ou exercício implementado.

Consulte os seguintes materiais para ajuda adicional:
- [Exemplo de README.md de repositório](misc/Template_README_Repositorio.md)
- [Exemplo de README.md para cada projeto](misc/Template_README_Projeto.md)
